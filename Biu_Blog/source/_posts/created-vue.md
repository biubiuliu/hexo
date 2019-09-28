---
title: vue如何新建一个项目
date: 2019-09-28 10:58:51
tags:
- vue
categories:
- 前端
---
## vue如何新建一个项目
####  第一步
下载安装[node](https://nodejs.org/zh-cn/)环境

下载完成后直接安装即可

自定义安装可能需要配置环境变量

安装完成后打开cmd命令行, 执行以下命令
```
node -v

npm -v
```
执行成功会显示对应的版本号

![markdown](https://www.mdeditor.com/images/logos/markdown.png "markdown")

####  第二步

如果之前有创建过vue项目, 那么你肯定安装过vue-cli 

```
vue list
```
![markdown](https://www.mdeditor.com/images/logos/markdown.png "markdown")

出现以下情况则可以省略 npm install vue-cli -g 这一步

![markdown](https://www.mdeditor.com/images/logos/markdown.png "markdown")

```
npm install vue-cli -g
```

然后执行 
```
vue init webpack  "项目名称"
```
![markdown](https://www.mdeditor.com/images/logos/markdown.png "markdown")

这时候文件已经创建完成

cd "项目名称"

然后执行
```
npm run dev
```
如果没有文件中没有下载依赖,可直接执行 npm i

npm i 是 npm install 的缩写

```
npm i 
```

好啦 ! 一个简单的vue 项目就创建成功啦 ! 



