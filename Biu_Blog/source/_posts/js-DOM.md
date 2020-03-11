---
title: HTML DOM
date: 2020-03-09 09:50:35
tags:
- 博客
categories:
- 前端
---

# JavaScript之神奇的DOM

文档对象模型（Document Object Model，简称DOM）将 web 页面与到脚本或编程语言连接起来，是W3C组织推荐的处理可扩展置标语言的标准编程接口。
在 HTML 语言中，标签可能拥有特性。当浏览器读取 HTML 文本并根据标签生成 DOM 对象，它会辨别标准化特性然后以此创建 DOM 属性。
![dom树](https://s2.ax1x.com/2020/03/10/8PwT0S.gif)

#### 特征

在DOM树中，有一个根节点，所有其他的节点都是根节点的后代。
![dom标签](https://s2.ax1x.com/2020/03/10/8iS3Pf.png)


#### 通过dom 我们能做什么?

##### 1. 增
```
document.createElement(element) //创建
document.appendChild(element) //添加
```
![新增dom](https://s2.ax1x.com/2020/03/10/8iCDit.png "新增dom")
###### 浏览器预览
![浏览器预览](https://s2.ax1x.com/2020/03/10/8iCXw9.png "浏览器预览")
##### 2. 删
```
document.removeChild(element)
document.replaceChild(new, old)
```
![删除dom](https://s2.ax1x.com/2020/03/10/8iisKS.png "删除dom")
###### 浏览器预览
![删除节点预览](https://s2.ax1x.com/2020/03/10/8iiBgf.png "删除节点预览")

##### 3. 查
```
document.getElementById(id)
document.getElementsByTagName(name)
document.getElementsByClassName(name)

```
![删除dom](https://s2.ax1x.com/2020/03/10/8ikiOU.png "查改dom")
###### 浏览器预览
![删除节点预览](https://s2.ax1x.com/2020/03/10/8ikClV.png "查改节点预览")
##### 4. 改
 上图
 
####  节点关系
```
<html>

  <head>
    <title>DOM Tutorial</title>
  </head>

  <body>
    <h1>DOM Lesson one</h1>
    <p>Hello world!</p>
  </body>

</html>
```
1. <html> 是根节点
2. <html> 没有父母
3. <html>是<head>和<body>的父
4. <head> 是大儿子 <html>
5. <body> 小儿子 <html>
