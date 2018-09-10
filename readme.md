
# SpringCloud环境搭建
   此项目环境为Spring Cloud Finchley版本
   [Finchley版本官方文档](http://cloud.spring.io/spring-cloud-static/Finchley.RELEASE/single/spring-cloud.html)
#### Eureka
   服务的注册与发现Eureka(项目块：eureka-server** 端口号：877*)
#### Eureka Client
   服务提供者 (项目块：eureka-hi** 端口号：876*)
#### 服务消费者 
   ###### RestTemplate+Ribbon
   服务消费者（rest+ribbon 项目块：service-ribbon** 端口号：878*）
   ###### Feign
   服务消费者（Feign 项目块：service-feign** 端口号：878*）
####  路由网关(zuul)
   路由网关(zuul)(项目块: service-hystrix** 端口号：878*)
####  路由网关(zuul)
