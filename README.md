## 技术栈

### 前端

前端基本借鉴 Yin 的云音乐

[地址]: https://github.com/Yin-Hongwei/music-website#music-website

项目，后端为自己实现

### 后端

**SpringBoot + MyBatis + Redis**

## 开发环境

JDK： jdk-1.8

mysql：8.0.2

redis：7.0

node：14.16.0

IDE：IntelliJ IDEA 2022、VSCode

## 下载运行

### 1、下载项目到本地

```bash
git clone https://github.com/Coco-001/WebMusic.git
```

### 2、修改配置文件

1）创建数据库
将 `music-website/music-server/sql` 文件夹中的 `tp_music.sql` 文件导入数据库。

2）修改用户名密码
修改 `music-website/music-server/src/main/resources/application.properties` 文件里的 `spring.datasource.username` 和 `spring.datasource.password`；

### 3、启动项目

- **启动管理端**：进入 music-server 文件夹，运行下面命令启动服务器

```js
// 方法一
导入 music-server 文件夹到 IDEA， 等待自动下载安装依赖， 点击 run 即可

// 方法二
./mvnw spring-boot:run

// 方法三
mvn spring-boot:run // 前提装了 maven
```

- **启动 redis**：直接在终端输入下面命令（必须先下载安装 Redis）

```
redis-server
```

- **启动客户端**：进入 music-client 目录，运行下面命令

```js
npm install // 安装依赖

npm run serve // 启动前台项目
```

- **启动管理端**：进入 music-manage 目录，运行下面命令

```js
npm install // 安装依赖

npm run serve // 启动后台管理项目
```
