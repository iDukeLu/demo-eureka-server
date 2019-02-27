# demo-eureka-server
Demo project for Spring Cloud Eureka Server

## 关于 eureka server 的配置文件
eureka server，即服务注册中心，更多的类似一个现成的产品，在大多数情况下，我们不需要修改它的配置信息。

## 高可用配置中心
#### 实现方式
高可用的服务注册中心实现非常简单，仅需：将 Eureka Server 作为服务与其他 Eureka Server 相互注册即可。

#### 打包方式
使用 -P 设置打包的环境
```
mvn clean package spring-boot:repackage -P manager1
```
