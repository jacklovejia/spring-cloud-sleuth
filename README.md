eureka-service 服务注册中心\
eureka-client 服务提供者\
eureka-feign-client 使用springcloud内置http工具调用服务\
eureka-ribbon-cline 使用声明式方式调用服务\
eureka-monitor-client\
eureka-zuul-client springcloud网关\
springboot-admin springbootadmin监控系统\
zipkin-server 分布式服务链路追踪\

springboot-admin springbootadmin监控系统\
    admin服务依赖直接看pom就可以\
    客户端, 也就是谁哪个服务需要springboot-admin监控\
    客户端依赖并且配置\
        pom 依赖\
         <dependency>\
                    <groupId>de.codecentric</groupId>\
                    <artifactId>spring-boot-admin-starter-client</artifactId>\
                    <version>1.5.5</version>\
          </dependency>\
        yml配置\
            spring:\
              boot:\
                admin:\
                  url: http://localhost:8000 # springbootadmin 地址\
        
          


