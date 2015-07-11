# Tomcat

Tomcat 服务器是一个免费且开放源代码的互联网应用服务器，属于轻量级应用服务器，在中小型系统和并发访问用户不是很多的场合下被普遍使用，是开发和调试 JSP 程序的首选。

本镜像源自于 Docker Hub 镜像 **[tutum/Tomcat](https://registry.hub.docker.com/u/tutum/tomcat/)**。

## 版本

当前版本 Tomcat 7.0.55

## 运行需求

最低 256 MB 内存

## 说明

容器启动后会自动创建一个具有所有权限的 `admin` 用户，并自动生成随机密码。你可以通过查看容器 log 获得密码，比如

```
========================================================================
You can now configure to this Tomcat server using:

    admin:1Bwjynh6rAb5

========================================================================
```

在上面的例子中，`1Bwjynh6rAb5` 就是 `admin` 用户的密码。

你可以用 `admin` 用户访问下面的地址配置 Tomcat:

* http://your-tomcat-url/manager/html

* http://your-tomcat-url/host-manager/html

如果你想为 `admin` 用户设置一个特定的密码，你可以设置环境变量 `TOMCAT_PASS` 为您需要的密码。


