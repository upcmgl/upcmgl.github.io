---
layout: post
title:  "怎么安装jekyll & ruby"
categories: jekyll
tags:  jekyll  
author: 马国蕾
---

* content
{:toc}


## 前言
本教程是说明如何在win10系统中安装jekyll 博客



##  安装步骤之第一步
首先去官网下载一个带devkit的rubyinstaller,下载链接：https://rubyinstaller.org/downloads/

注：不是很清楚有没有被墙，如果不能访问可以联系我。

2.打开命令行工具输入

输入“ruby -v”、“gem -v”检测有没有安装成功。

安装成功应该会正常显示版本。

3.输入“gem install jekyll”

等待一会，便会出现下面这样的界面（太长了，只截一部分），表示安装成功 ：



4.检测是否安装成功，输入“jekyll -v”

显示版本即表示安装成功。

##  安装步骤之第二步
使用Jekyll创建你的博客站点
jekyll new blog  #创建你的站点
控制台可以看见类似 New jekyll site installed in /home/user/blog.的提示

开启Jekyll服务
cd blog         #进入blog目录,记得一定要进入创建的目录，否则服务无法开启
jekyll serve      #启动你的http服务
注：
如果启动后发现错误
  Dependency Error: Yikes! It looks like you don't have jekyll-paginate or one of its dependencies installed. In order to use Jekyll as currently configured, you'll need to install this gem. If you've run Jekyll with `bundle exec`, ensure that you have included the jekyll-paginate gem in your Gemfile as well. The full error message from Ruby is: 'cannot load such file -- jekyll-paginate' If you run into trouble, you can find helpful resources at https://jekyllrb.com/help/!
可以使用gem install jekyll-paginate

本地服务开启后，Jekyll服务默认端口是4000，所以我打开浏览器，输入：http://localhost:4000 即可访问
我的地址是这个： Server address: http://127.0.0.1:4001/  在浏览器中就可以使用该地址进行访问。