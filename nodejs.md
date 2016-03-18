# 安装 Node.js 和 npm

### 获取资源
```shell
# 4.x
curl --silent --location https://rpm.nodesource.com/setup_4.x | bash -
```
```shell
# 5.x
curl --silent --location https://rpm.nodesource.com/setup_5.x | bash -
```
```shell
# 0.10
curl --silent --location https://rpm.nodesource.com/setup | bash -
```


### 安装 MongoDB
```shell
yum install -y nodejs
```

### 其他 -- 编译工具
```shell
yum install gcc-c++ make
# or: yum groupinstall 'Development Tools'
```

### 测试是否安装成功

```shell
node -v 
# v4.4.0
npm -v
# 2.14.20
```


[官网链接](https://nodejs.org/en/download/package-manager/ "官网链接")
