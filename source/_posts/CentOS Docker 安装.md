---
title: '''CentOS Docker 安装'''
date: 2020-08-01 08:59:07
comments: true
categories: #分类 
      - 运维
tags:  #标签
     - docker
---
CentOS操作系统环境下安装Docker
<!--more-->

## 使用官方脚本自动安装

安装命令如下:
``` bash
curl -fsSL https://get.docker.com | bash -s docker --mirror Aliyun
```

也可以使用国内 daocloud 一键安装命令：
``` bash
curl -sSL https://get.daocloud.io/docker | sh
```
安装 Docker Engine-Community:
``` bash
$ sudo yum install docker-ce docker-ce-cli containerd.io
```
如果提示您接受 GPG 密钥，请选是。

启动docker：
``` bash
$ sudo systemctl start docker
```
通过运行 hello-world 映像来验证是否正确安装了 Docker Engine-Community。
``` bash
$ sudo docker run hello-world
```
