---
title: git 的入门使用
date: 2020-02-19 10:55:00
tags:
---

## 下载安装 git
git 下载地址：https://git-scm.com/downloads

配置用户名
```Shell
git config --global user.name "Your Name"
```

设置邮箱
```Shell
git config --global user.email "your_email@example.com"
```

列出当前用户的全局 Git 配置信息
```Shell
git config --global --list
```
>user.email=your_email@example.com  
>user.name=Your Name


## 连接 GitHub

### 创建 SSH 密钥
```shell
ssh-keygen -t rsa -C "your_email@example.com"
```

> id_rsa 私钥保存在本地  
> id_rsa.pub 公钥复制到远程

### 查看公钥
```shell
cat ~/.ssh/id_rsa.pub
```
> ssh-rsa ****** your_email@example.com

复制公钥到GitHub

### 测试 SSH  是否连接到 GitHub
```shell
ssh -T git@github.com
```
>Hi Your Name! You've successfully authenticated, but GitHub does not provide shell access.
