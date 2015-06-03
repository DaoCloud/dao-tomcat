# Tomcat

Tomcat 服务器是一个免费的开放源代码的Web 应用服务器，属于轻量级应用服务器，在中小型系统和并发访问用户不是很多的场合下被普遍使用，是开发和调试JSP 程序的首选。

本镜像源自于DockerHub镜像[tutum/Tomcat](https://registry.hub.docker.com/u/tutum/tomcat/)。

## 版本

当前版本 Tomcat 7.0.55

## 运行需求

256M内存及以上

## 说明

容器启动后会自动创建一个具有所有权限的admin用户，并自动生成随机密码。你可以通过查看容器log获得密码，比如

> => Creating and admin user with a random password in Tomcat

> => Done!

> ========================================================================

> You can now configure to this Tomcat server using:

>     admin:1Bwjynh6rAb5

> ========================================================================

在上面的例子中，*1Bwjynh6rAb5* 就是admin用户的密码。

你可以用admin用户访问下面的地址配置Tomcat:

－ http://your-tomcat-url/manager/html

－ http://your-tomcat-url/host-manager/html

如果你想为admin用户设置一个特定的密码，你可以设置环境变量 *TOMCAT_PASS* 为您需要的密码。


