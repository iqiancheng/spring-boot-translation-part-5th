# 第五章 Spring Boot Actuator：生产就绪(Production-ready) 功能

`Spring Boot` 自带了一些很有用的功能来帮助开发者监控和管理发布在生产环境的应用程序。你可以选择开启HTTP端口利用JMX监控，或者通过远程Shell（SSH或Telnet）方式来对你的 Spring-Boot 应用进行自动化管理：审计、健康检查和性能指标采集。

例如，HTTP环境下，访问 `/health` 路径即可查询当前环境的磁盘空间，应用和数据库的状态等；访问 `/metrics` 路径即可查询当前jvm的内存使用情况，线程池的状态等。

Http 端执行器(Actuator) 只适用于基于 `Spring MVC` 的应用。尤其注意 `Jersey `（一个JAX-RS的实现，类似于Spring MVC） 是不支持的。能够使用 `Spring Boot Actuator` 特性的前提是你的项目必须是使用了 Spring MVC 框架。


