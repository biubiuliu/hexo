---
title: blog
date: 2019-10-09 09:50:35
tags:
- 博客
---
## 如何利用 github 搭建一个属于自己的博客

首先你需要做以下准备

_node环境
github 账号或者 gitee账号
hexo_

这里以gitee为例

#### 第一步 创建仓库
![新建仓库](http://pykvjcrlq.bkt.clouddn.com/crated.png "新建仓库")

这里与github有所不同

![设置gitee.io](http://pykvjcrlq.bkt.clouddn.com/gitee_page.png "设置gitee.io")


#### 第二步 安装hexo
打开 shell 终端，输入命令`npm install -g hexo`
成功之后初始化hexo，输入命令`hexo init`

生成目录
![初始化hexo](http://pykvjcrlq.bkt.clouddn.com/hexo_init.png "初始化hexo")

然后关联gitee地址
![关联gitee](http://pykvjcrlq.bkt.clouddn.com/gitee_url.png  "初始化hexo")


#### 第三步  发布

发布之前配置在_config.yml中配置

```

deploy:
  type: git
  repo: https://gitee.com/biubiuliu/blog.git
  branch: master
```

发布到Gitee
输入命令`npm install hexo-deployer-git --save` 安装自动部署发布工具
输入命令`hexo g ` 生成 public文件 里面是 静态html
输入命令`hexo s ` 启动本地服务, 本地预览
输入命令`hexo clean && hexo g && hexo d` 发布博客，首次发布需要在shell中输入账号和密码。

如果出现以下情况
![blog样式错误](http://pykvjcrlq.bkt.clouddn.com/blog_index.png  "blog样式错误")

则需要在_config.yml中配置下博客地址和路径：

```
url: https://biubiuliu.gitee.io/blog
root: /blog

```

点击生成的地址访问
![访问](http://pykvjcrlq.bkt.clouddn.com/gitee_page.png "访问")


在线效果如下
![效果](http://pykvjcrlq.bkt.clouddn.com/online_blog.png "效果")

##### 到这一步我们一个简单的博客系统就搭建完成了


 接下来玩一下升级版的

 ### 更改主题

 以上的默认主题, 真的有难看,逼格不够高

 我们进入[hexo](http://pykvjcrlq.bkt.clouddn.com/hexo_theme.png)选择自己喜欢的主题
 然后将其clone 或者直接下载zip
![ 主题](http://pykvjcrlq.bkt.clouddn.com/hexo_theme.png)

将clone 或者 解压后的zip 文件放入themes文件夹中
 
![themes](http://pykvjcrlq.bkt.clouddn.com/hexo_file_themes.png)

打开config.yml文件 更改主题文件名

找到这一段
```
# Extensions
## Plugins: https://hexo.io/plugins/
## Themes: https://hexo.io/themes/
theme: landscape
```
更改为
```
# Extensions
## Plugins: https://hexo.io/plugins/
## Themes: https://hexo.io/themes/
theme: hexo-theme-geektutu-master
```
然后部署就OK了

![最终效果](http://pykvjcrlq.bkt.clouddn.com/blog_view.png)
