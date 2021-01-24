# Sentinel持久化到Nacos配置中心
基于Sentinel 1.8.0改造。
将authority（授权规则）、degrade（降级规则）、flow（流控规则）、param（热点规则）、system（系统规则）五种规则持久化到Nacos中。
另外还增加网关的两个（api分组，限流）

# 改造步骤
可前往博客查看：https://blog.visionki.com/index.php/archives/101/

# 使用方法
- 拉取源码。
- 修改`sentinel-dashboard`模块下的`application.properties`文件中Nacos相关配置。
- 前往源码根目录执行`mvn package -DskipTests`打包。
- 运行`sentinel-dashboard/target`文件夹下的jar包。