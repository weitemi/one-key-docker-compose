# one-key-docker-compose
Windows、Linux、Mac一键docker-compose安装脚本

## 使用教程

### 下载项目后进入需要安装的目录执行命令：
```
docker-compose up -d
```
## 介绍

### consul

Consul是一个服务网格解决方案，提供了一个功能齐全的控制平面，具有服务发现、配置和分段功能。

常用于服务发现和配置中心
### jaeger

Jaeger 是一种软件，可用于监控和解决互连软件组件（称为微服务）上存在的问题。 多个微服务相互通信以完成单个软件功能。 开发人员使用Jaeger 可视化这些微服务交互中的事件链，以便在出现问题时将其隔离。

常用于分布式链路跟踪

安装前

修改docker-compose.yml的宿主机IP

### kafaka

Kafka是一个分布式流处理系统，流处理系统使它可以像消息队列一样publish或者subscribe消息，分布式提供了容错性，并发处理消息的机制。

常用于消息队列

安装前

修改docker-compose.yml的宿主机IP

### mysql

MySQL是一个关系型数据库管理系统，由瑞典MySQL AB 公司开发，属于Oracle旗下产品。 MySQL是最流行的关系型数据库管理系统之一，在WEB 应用方面，MySQL是最好的RDBMS (Relational Database Management System，关系数据库管理系统)应用软件之一。

安装前

修改docker-compose.yml的mysql数据库root密码

### nacos

Nacos /nɑ:kəʊs/ 是Dynamic Naming and Configuration Service的首字母简称，一个更易于构建云原生应用的动态服务发现、配置管理和服务管理平台。 Nacos 致力于帮助您发现、配置和管理微服务。

安装前

1、修改docker-compose.yml的MYSQL主机IP

2、修改配置文件的数据连接URL

3、在数据库中导入初始数据（导入init-nacos.sql）

### php

使用docker-compose一键搭建本地php开发环境
PHP（全称：PHP: Hypertext Preprocessor，即“PHP：超文本预处理器”）是一种开源的通用计算机脚本语言，尤其适用于网络开发并可嵌入HTML中使用。 PHP的语法借鉴吸收C语言、Java和Perl等流行计算机语言的特点，易于一般程序员学习。

安装前

1、修改php项目的运行目录（即index.php）

2、修改docker-compose.yml的项目名称

### rabbitmq

RabbitMQ 是一个开源的AMQP 实现，服务器端用Erlang 语言编写，支持多种客户端，如：Python、Ruby、.NET、Java、JMS、C、PHP、ActionScript、XMPP、STOMP 等，支持AJAX。 用于在分布式系统中存储转发消息，在易用性、扩展性、高可用性等方面表现不俗。


## 注意事项

### 所有镜像均为官方镜像，默认数据、配置、日志都保存在docker-compose运行的文件夹下。
