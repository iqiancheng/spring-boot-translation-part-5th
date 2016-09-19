# 第五章 Spring Boot Actuator：生产就绪(Production-ready) 功能

`Spring Boot` 自带了一些额外的功能来帮助开发者监控和管理发布在生产环境的应用程序。你可以选择开启HTTP端口利用JMX监控，或者通过远程Shell（SSH或Telnet）方式来对你的 Spring-Boot 应用 进行自动化管理、审计和健康指标采集。

Http 端执行器(Actuator) 只适用于基于 `Spring MVC` 的应用。尤其注意 `Jersey `（一个JAX-RS的实现，类似于Spring MVC） 是不支持的，除非你的项目是使用 Spring MVC。


