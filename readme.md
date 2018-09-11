
# SpringCloud环境搭建
   ##### write author : weipeng
   此项目环境为Spring Cloud Finchley版本
   [Finchley版本官方文档](http://cloud.spring.io/spring-cloud-static/Finchley.RELEASE/single/spring-cloud.html)
#### Eureka
   服务的注册与发现Eureka(项目模块：eureka-server** 端口号：877*)
#### Eureka Client
   服务提供者 (项目模块：eureka-hi** 端口号：876*)
#### 服务消费者 
   ###### RestTemplate+Ribbon
   服务消费者（rest+ribbon 项目模块：service-ribbon** 端口号：878*）
   ###### Feign
   服务消费者（Feign 项目模块：service-feign** 端口号：878*）
####  断路器(hystrix)
   断路器(hystrix)(项目模块: service-hystrix** 端口号：878*)
####  路由网关(zuul)
   路由网关(zuul)(项目模块：service-zuul** 端口号：879*)
   zuul不仅只是路由，并且还能过滤，做一些安全验证(继承ZuulFilter).
#### 分布式配置中心(Spring Cloud Config)
    <dependency>
   			<groupId>org.springframework.cloud</groupId>
   			<artifactId>spring-cloud-config-server</artifactId>
   			<version>1.3.3.RELEASE</version>
   	</dependency>
   	<parent>
    		<groupId>org.springframework.boot</groupId>
    		<artifactId>spring-boot-starter-parent</artifactId>
    		<version>1.5.3.RELEASE</version>
    		<relativePath/> <!-- lookup parent from repository -->
    	</parent>
  所加依赖如上所示，这里会有版本冲突的问题
  分布式配置中心(Spring Cloud Config)(项目模块: config-server 端口号：881*)
  