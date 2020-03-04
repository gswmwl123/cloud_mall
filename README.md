# mallcloud-platform



  * 账号密码：admin/123456
  * 应用监控账号密码：admin/admin
  * 配置中心账号密码：nacos/nacos
  * APM监控账号密码：admin/admin
  * Grafana账号：mall/mall
  * txlcn事务管理器密码：admin
  * 任务管理账号密码：admin/123456

* 前后端分离的企业级微服务架构
* 基于`Spring Boot 2.0.X`、`Spring Cloud Finchley`和`Spring Cloud Alibaba`
* 深度定制`Spring Security`真正实现了基于`RBAC`、`jwt`和`oauth2`的无状态统一权限认证的解决方案
* 提供应用管理，方便第三方系统接入
* 引入组件化的思想实现高内聚低耦合，项目代码简洁注释丰富上手容易
* 注重代码规范，严格控制包依赖，每个工程基本都是最小依赖
* 非常适合学习和企业中使用

>

mallcloud -- 父项目，公共依赖
│  ├─mall-business -- 业务模块一级工程
│  │  ├─user-center -- 用户中心[7000]
│  │  ├─file-center -- 文件中心[5000]
│  │  ├─member-center -- 会员中心[7001]
│  │  ├─goods-center -- 商品中心[7002]
│  │  ├─order-center -- 订单中心[7003]
│  │  ├─marking-center -- 营销中心[7004]
│  │─mall-commons -- 通用工具一级工程
│  │  ├─mall-auth-client-spring-boot-starter -- 封装spring security client端的通用操作逻辑
│  │  ├─mall-common-spring-boot-starter -- 封装通用操作逻辑
│  │  ├─mall-db-spring-boot-starter -- 封装数据库通用操作逻辑
│  │  ├─mall-log-spring-boot-starter -- 封装log通用操作逻辑
│  │  ├─mall-redis-spring-boot-starter -- 封装Redis通用操作逻辑
│  │  ├─mall-ribbon-spring-boot-starter -- 封装Ribbon和Feign的通用操作逻辑
│  │  ├─mall-sentinel-spring-boot-starter -- 封装Sentinel的通用操作逻辑
│  │  ├─mall-swagger2-spring-boot-starter -- 封装Swagger通用操作逻辑
│  ├─mall-config -- 配置中心
│  ├─mall-doc -- 项目文档
│  ├─mall-gateway -- api网关一级工程
│  │  ├─zuul-gateway -- netflix-zuul[8080]
│  ├─mall-job -- 分布式任务调度一级工程
│  │  ├─job-admin -- 任务管理器[8081]
│  │  ├─job-core -- 任务调度核心代码
│  │  ├─job-executor-samples -- 任务执行者executor样例[8082]
│  ├─mall-monitor -- 监控一级工程
│  │  ├─sc-admin -- 应用监控[6500]
│  │  ├─log-center -- 日志中心[6200]
│  ├─mall-uaa -- spring-security认证中心[8000]
│  ├─mall-register -- 注册中心Nacos[8848]
│  ├─mall-transaction -- 事务一级工程
│  │  ├─txlcn-tm -- tx-lcn事务管理器[7970]
│  ├─mall-demo -- demo一级工程
│  │  ├─txlcn-demo -- txlcn的demo
│  │  ├─sharding-jdbc-demo -- sharding-jdbc的demo
```

