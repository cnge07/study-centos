# 安装 MongoDB

### 创建 repo 文件 （只支持 x64）
```shell
vi /etc/yum.repos.d/mongodb-org-3.2.repo
```

#### 文件内容：
```shell
f[mongodb-org-3.2]
name=MongoDB Repository
baseurl=https://repo.mongodb.org/yum/redhat/$releasever/mongodb-org/3.2/x86_64/
gpgcheck=1
enabled=1
```

### 安装 MongoDB
```shell
yum install -y mongodb-org
```

#### 安装完成包含下列服务

- mongodb-org
- mongodb-org-server
- mongodb-org-mongos
- mongodb-org-shell
- mongodb-org-tools

默认配置文件位置：/etc/mongod.conf
默认日志位置： /var/log/mongodb/mongod.log
默认数据位置： /var/lib/mongo
默认绑定 ip ： 127.0.0.1
默认端口号： 27017

### 常用命令

开机启动 mongodb
```shell
chkconfig mongod on
```

停止 mongodb
```shell
service mongod stop
```

重启 mongodb
```shell
service mongod restart
```

[官网链接](https://docs.mongodb.org/master/tutorial/install-mongodb-on-red-hat/ "官网链接")
