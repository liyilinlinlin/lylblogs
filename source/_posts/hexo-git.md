---
title: hexo 博客搭建之路--部署到github上
---

# 前言
    在此之前你应该有一个属于自己的github账号

## 创建一个新的repository
    打开你的GitHub首页，在左边有一个 New repository 按钮，点击创建一个新的repository，例如我的名字是 liyilinlinlin ，那么我的repository名字就是 liyilinlinlin.gitbub.io
    
    
![](.\..\images\newimg.png)

**注意**

    一定要以 你的github用户名.github.io 创建，否则会出现404错误

## 将本地文件部署到GitHub账号中

    编辑站点配置文件 _config.yml 中的deploy

```
# Deployment
## Docs: https://hexo.io/docs/deployment.html
deploy:
  type: git
  repository: https://github.com/liyilinlinlin/liyilinlinlin.github.io.git
  // https://github.com/你的用户名/你的用户名.github.io.git
  branch: master

  //.yml文件对格式规范要求很严格，type: repository: branch: 前面有两个空格，冒号后面都有一个空格。

```

## 执行一下命令完成部署

```

hexo g  //用于保存修改的文件

hexo d  //用于上传到github上

```

**注意**

1、 若没有设置GitHub上的ssh，则会导致失败，需提前配置好ssh
2、 使用 hexo g 须在hexo的根目录下使用
3、 若执行 hexo d ，提示 ERROR Deployer not found: git，需安装 hexo-deployer-git 依赖包，
    npm install hexo-deployer
4、当你执行 hexo d 的时候，出现提示框让你输入github用户名和密码，只要输入正确，上传就可以了
5、现在博客就部署成功了，在浏览器上访问 [liyilinlinlin.github.io](https://liyilinlinlin.github.io)就行了