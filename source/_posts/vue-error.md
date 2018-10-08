---
title: vue 项目搭建遇到的问题
tags:
    - vue
    - npm
---

### 问题一

当出现一下错误时
```
npm ERR! code ELIFECYCLEnpm ERR! errno 1npm ERR! chromedriver@2.41.0 install: `node install.js`
npm ERR! Exit status 1npm ERR!npm ERR! Failed at the chromedriver@2.41.0 install script.npm ERR! This is probably not a problem with npm. There is likely additional logging output above.

```
在所在目录执行
     npm install chromedriver --chromedriver_cdnurl=http://cdn.npm.taobao.org/dist/chromedriver 即可