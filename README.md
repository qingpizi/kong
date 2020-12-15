### 一、介绍
Kong环境搭建，以及插件开发框架。

### 二、文件结构
```
|---conf
|   |---kong.conf.default  //kong默认配置
|   |---kong.logrotate     //日志分割
|---logs                   //日志存放目录
|---plugin                 //自定义插件目录
|   |---kong                
|   |   |---plugins
|   |   |   |---插件目录
|   |   |   |---...
|---.env.example            //docker-compose.yaml参数默认配置
|---.gitignore 
|---docker-compose.yaml     //搭建环境配置
|---README.md               
```
### 环境安装

1.复制Kong配置文件，按需进行调整
```
cp conf/kong.conf.default conf/kong.conf
```
2.复制docker-compose.yaml变量配置文件，按需进行调整
```
cp .env.example .env
```
3.执行环境构建
```
 docker-compose up -d
```