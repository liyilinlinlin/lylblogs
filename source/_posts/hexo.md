---
title: hexo 博客搭建之路
---

# 部署环境

git (从官网上下载就行)
node.js (同上)
windows

## git 的基本配置

配置用户名（先在github上注册一个账号）

```
git config --global user.name 'yourname'
git config --global user.email 'youremail'
```

ssh key 生成

```
ssh-keyhen -t rsa -C 'youremail'
//生成密匙后，会显示文件地址，将密匙复制到GitHub中

git config --list
//可以查看用户名和邮箱
```
安装hexo命令行

```
npm install -g hexo-cli
hexo init 文件夹名称  //初始化文件
cd 文件   //进入文件
npm install
hexo server  //启动服务
```
访问http://loaclhost:4000

