# 拼团旅游信息管理平台

## 一、拼团旅游信息网

### 1、依赖环境：

* jdk 8
* mysql 8.0 以上版本
* redis 无版本要求
* kafka_2.12-2.8.1

### 2、项目工程结构

### 3、项目配置

resources目录下的application.properties文件中，保存着项目的相关配置

* 其中的数据源配置用于配置连接数据库相关配置项
* Mail配置用于配置发送邮件的邮箱相关配置
* Redis配置用于配置连接Redis相关
* 常量配置保存着一些默认的常量配置数据，如用户默认的头像等
* 腾讯云相关配置用于配置连接腾讯云对象存储所用，如何使用可查看腾讯对象存储官方文档

### 4、环境启动

* 启动zookeeper

在IDEA中打开Terminal，在窗口中进入到kafka的安装目录，然后执行命令。

```shell
bin\windows\zookeeper-server-start.bat config\zookeeper.properties
```

![image-20230525221701889](C:/Users/17271/AppData/Roaming/Typora/typora-user-images/image-20230525221701889.png)

* 启动kafka

打开一个新的窗口，启动kafka

```shell
bin\windows\kafka-server-start.bat config\server.properties
```

![image-20230525222201655](C:/Users/17271/AppData/Roaming/Typora/typora-user-images/image-20230525222201655.png)

之后启动redis和mysql的服务就可以运行了

> 注意：如果在启动kafka的时候启动失败，需要先进入到kafka的日志输入的目录中将里面的文件全部删除，然后重新启动就可以了

### 5、项目启动

项目启动后，成功打印出SUCCESS字样说明启动成功，之后点打印出的本地访问地址，就可以打开浏览器访问项目了

### 6、项目功能介绍

* 首页：热点推荐、景点推荐
* 景点

### 7、系统展示

### 8、技术介绍

## 二、拼团旅游信息管理后台