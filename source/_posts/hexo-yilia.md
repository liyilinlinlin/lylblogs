---
title: hexo 博客搭建之路-yilia主题
tags:
    - hexo
    - yilia
---
## 开始

```
$ git clone https://github.com/litten/hexo-theme-yilia.git themes/yilia
```

### 配置

修改站点配置文件config.yml中的theme。。  theme: yilia

## 配置yilia主题

**注意**
  ---格式一定要正确，否则页面会显示缺少模块

```
// 下载 hexo-generator-json-content
npm install hexo-generator-json-content

//在站点配置文件中添加
jsonContent:
  meta: false
  pages: false
  posts:
    title: true
    date: true
    path: true
    text: false
    raw: false
    content: false
    slug: false
    updated: false
    comments: false
    link: false
    permalink: false
    excerpt: false
    categories: false
    tags: true

```

### 关于图片显示问题

在yilia主题中，不遵循相对路径，它是以source文件夹为根目录的。
例如：配置yilia主题的头像链接
```
//在source文件夹下新建images文件夹存入图片pig.jpg
//在yilia主题配置文件_config.yml中
avatar: /images/pig.jpg
```
**注意**
保存图片的文件夹不能放在_posts文件夹下，或以特殊符号开头的文件夹下，否则图爿路径不正确
