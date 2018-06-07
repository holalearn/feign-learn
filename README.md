## 》基本配置
```
// feign-consumer
一、引入feign依赖
二、通过@EnableFeignClients开启Spring Cloud Feign的支持
三、 1）定义接口，通过@FeignClient注解指定服务名来绑定服务
三、 2）使用Spring MVC注解绑定服务提供的某一个REST接口
四、将Feign服务注入
五、定义自身服务名
六、配置服务注册中心
```

## 》》继承优化
```
// hello-service-api
一、创建需要复用的DTO和接口
二、使用Spring MVC的注解，引用spring-boot-starter-web依赖

// hello-service
三、使用api和DTO，添加对hello-service-api的依赖
四、Controller类继承并实现复用接口

// feign-consumer
五、使用api和DTO，添加对hello-service-api的依赖
六、feign接口继承复用接口
```
