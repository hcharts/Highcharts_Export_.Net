Highcharts_Export_.Net
=====================

# Highcharts 导出服务.Net版

## 安装
### 一、安装依赖
```sh
$ yum -y install java-1.7.0-openjdk
$ yum -y install gcc-c++
```

### 二、搭建zookeeper
1.新建目录
```sh
$ mkdir -p /data/apps
$ mkdir -p /data/logs
$ mkdir -p /data/programfiles
```

2.下载[zookeeper](http://www.apache.org/dyn/closer.cgi/zookeeper/)，推荐下载3.4.5版本
```sh
$ cd /data/programfiles
$ wget http://mirror.bit.edu.cn/apache/zookeeper/zookeeper-3.4.5/zookeeper-3.4.5.tar.gz
$ tar -xvf zookeeper-3.4.5.tar.gz -C ./
```
3.启动zookeeper(zookeeper配置在这里不做详细介绍)
```sh
$ cp /data/programfiles/zookeeper-3.4.5/conf/zoo_sample.cfg /data/programfiles/zookeeper-3.4.5/conf/zoo.cfg
$ cd /data/programfiles/zookeeper-3.4.5/bin
$ ./zkServer.sh start
```
