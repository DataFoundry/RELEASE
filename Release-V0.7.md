# RELEASE 0.7
##页面
DataFoundry（域名：https://lab.dataos.io）

##CLI客户端
oc login https://dev.dataos.io:8443
 
##账号
DataFoundry已进入内测阶段，有账号的同事可登陆https://lab.dataos.io 进行试用；

如需账号申请，请发以下内容邮件至LDP运营部的李靖，邮箱：lijing9@asiainfo.com 

##客户端下载　

https://s3.cn-north-1.amazonaws.com.cn/datafoundry/client/linux-32bit.tar.gz

https://s3.cn-north-1.amazonaws.com.cn/datafoundry/client/linux-64bit.tar.gz

https://s3.cn-north-1.amazonaws.com.cn/datafoundry/client/mac.zip

https://s3.cn-north-1.amazonaws.com.cn/datafoundry/client/windows.zip

##客户端命令变更
- oc new-backingserviceinstance命令更新为oc new-instance，支持创建后端服务实例以及用户自定义后端服务实例。
可使用oc new-instance -h查看使用帮助：

```
Create a new BackingService instance

This command will try to create a backing service instance.

Usage:
  oc new-instance NAME [options]

Examples:
# Create a backingservice instance via backingservice
  $ oc new-instance mysql-instance --service=myslql --plan=shared

  # Create a user-provided-service
  $ oc new-instance redis-instance -p host=redis.somedomain.com -p port=6379 -p password=H3IIOw0R1D

Options:
  -p, --parameters=[]: Specify key value pairs of env variables for User-Provided-Service.
      --plan='': BackingService Plan Name
      --service='': BackingService Name

Use "oc options" for a list of global command-line options (applies to all commands).
```

- 系统后端服务实例以及用户自定义后端服务实例与服务绑定操作一致，使用oc bind操作。可用oc bind --h 查看使用帮助。

##新增功能
编号 | 一级功能 | 二级功能 | 三级功能 
----- | ----- | ----- | ----- 
1 | 用户中心 |  
2	|  | 用户注册与登录	　
3	 |  |  | 注册	
4	 |  | 组织管理
5	 |  |  | 创建组织
6	 |  |  | 成员邀请
7	 |  | 组织信息
8	 |  | 用户信息
9 | 信息中心

##后端支持服务 

序号 | 后端服务名称 | 版本 
----- | ----- | ----- 
1 | Kettle | v5.0.1
2 | NiFi | v0.6.1
3 | TensorFlow | v0.8.0
4 | AzureDocumentDB | 
5 | AzureStorageBlob | 
6 | AzureServiceBus |  
7 | AzureRedisCacheService | 	
8 | Mysql | 
9 | ZooKeeper | v3.4.8
10 | ETCD | v2.3.0
11 | Redis | v2.8
12 | Cassandra | v3.4
13 | Spark | v1.5.2
14 | Storm | v0.9.2
15 | Kafka | v0.9.0
16 | RabbitMQ | v3.6.1
17 | PostgreSQL | 	
18 | MongoDB | 
19 | Greenplum | 
20 | Oracle | v11.2
21 | Oracle Cloud | v11.2
22 | HBasevv1.1.2
23 | HDFS | v2.7.1

##周边设施
- 私有代码仓库：https://code.dataos.io
- 公共镜像仓库：https://registry.dataos.io
 
##沟通交流
在内测过程中，如有任何问题，可以通过以下三种渠道与我们交流，我们会有专人及时回复：
- 1、 可以在DataFoundry交流群中提问；
- 2、 在DataFoundry平台的DaoVoice中提问；
- 3、 在github这个地址里面提issue：https://github.com/asiainfoLDP/datafoundry-troubleshooting/issues
 
 


