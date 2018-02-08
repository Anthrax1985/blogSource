---
title: 体验hexo
date: 2017-08-17 17:35:23
tags: 
- hexo 
- demo
---

# 体验Hexo

所谓体验hexo，其实也就是自己对文档的再理解的过程。
下面把一些例子，记录下来，方便以后回忆


## Ⅰ.框架的构成 
hexo属于静态的blog框架，其主要的组成为
{% img structimage /img/hexo体验/hexo结构.png 284 399 [hexo结构图片] %}

接下来通过理解各个组成部分来掌握hexo

### 1.scaffoads(脚手架）

就和其字面意思一样，是为了快速生成某种固定layout，预先设置的模板内容。
在通过命令来新建文章时，通过设定的layout内容快速的寻找固定的模式，来生成文章。
{% codeblock %}
hexo new layout postName
{% endcodeblock %}


### 2.source(源文件)

这个文件夹就是整个hexo的核心，存放源文件的地方。
按照功能来划分3种类型的文件夹
* Post 
    正式发布的文件，通过*hexo g*来生成静态发布内容
* Draft 
    草稿箱 不能通过*hexo g*来生成内容
* Custom 
    自定义文件夹，通过*hexo g*来生成静态发布内容。


### 3.theme（主题）

为了显示不同的页面布局、我们可以通过自定义主题、或者引用别人主题的方式来
定制自己的hexo样式。


### 4.config.yaml(配置文件)

已经预设了hexo支持的配置项，只要简单的配置内容即可定制自己的blog




## Ⅱ.实际使用

### 1.环境配置
参考官方文档、百度一些文章就能完成，我这里就不重复造轮子

### 2.日常使用
对于日常写作来说、只要记住以下的命令基本就能运作起来。
{% codeblock 创建文章新文章 %}
hexo new layout postname
{% endcodeblock%}
{% codeblock 生成静态文件 %}
hexo g
{% endcodeblock%}
{% codeblock 本地预览服务器启动 %}
hexo server
{% endcodeblock%}
{% codeblock 部署 %}
hexo d
{% endcodeblock%}