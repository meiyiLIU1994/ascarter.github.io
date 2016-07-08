---
layout: post
title: 如何制作个人网站by刘美亿
date: '2014-06-30 10:22:40'
---

步骤：

新建动态网页工程---搭载服务器---在WebContent包中新建Views Floder---将模板导入---在html后缀的文件中修改页面显示以及跳转---css后缀的文件修改布局和大小---svg后缀文件设置插入的矢量图形


（1）基本模板搭建：这里可以自己搭建，最初的话，恩，像我们这次，都是直接用的模板。参考Bootstrap中文网 http://v3.bootcss.com/getting-started/

（2）导航条：在Eclipse里面通过对组件的设置，创建面板，设计导航条。参考Bootstrap中文网 http://v3.bootcss.com/components/#navbar

（3）轮播：使用Javascript的插件Carousel。参考Bootstrap中文网 http://v3.bootcss.com/css/#grid  

（4）内容布局：根据模板，对内容以及字体进行制作。

     利用全局CSS样式构造栅格系统，参考Bootstrap中文网 http://v3.bootcss.com/css/#grid

     Bootstrap 提供了一套响应式、移动设备优先的流式栅格系统，随着屏幕或视口（viewport）尺寸的增加，系统会自动分为最多12列。

     它包含了易于使用的预定义类，还有强大的mixin 用于生成更具语义的布局。

     Bootstrap把页面等分为12列，你可以将你的内容放入任意行中；

     比如可以（4：4：4）也可以（4：3：2）总之相加不要超过12，当屏幕变小后原来一行4：4：4；变为了三行，每行占满屏幕。

（5）标签页：同样可以使用Javascript插件制作标签页，参考Bootstrap中文网 http://v3.bootcss.com/css/#grid  

（6）版权信息：这个在模板的基础上改一改就行了，大家都差不多的。


根据我在模板基础上完成个人网站，有几个修改点以及注意事项：

（1）meta charset="utf-8" 如果网页出现中文，需要设置html5的中文编码，否则会出现乱码。

（2）title Curriculum Vitae of　Liu Meiyi /title   设置网站左上角的那个标题。

（3）li  a class="btn" href="https://meiyiliu1994.github.io/archive.html" Blog /a  /li  Blog按钮指向博客。

（4）a class="btn btn-action btn-lg"  href="https://meiyiliu1994.github.io/archive.html" role="button">CONTACT ME /a  CONTACT ME 指向博客地址。

（5）#符号表示本标签指向本页面。

（6）Copyright &copy 2016,  Designed by a href="https://meiyiliu1994.github.io/archive.html" rel="designer">Liu Meiyi /a>  将LiuMeiyi指向博客地址。

（7）h1 表示一级标题，一般作为题目； h2 二级标题；table 制表符，对齐方式左对齐；td 表示表格横行内容；width表示宽度；p 是表示插入段落文章内容。

（8） p  利用语句 img src="****.jpg" alt="" class="img-rounded pull-right" width="200"    插入图片 环绕方式 宽度为200。

推荐工具：
（1）w3schools.com：是最受欢迎的前端技术教程网站，国内的中文翻译版本十分陈旧。可以在网上找个镜像，希望英文好的同学直接去看原版教程吧！

（2）Bootstrap优站精选频道：收集了众多基于 Bootstrap 构建、设计精美的、有创意的网站。

（3）Buttons CSS按钮样式库：一个基于 Sass 和 Compass 构建的CSS按钮（button）样式库，图标采用的是Font Awesome，可以和Bootstrap融合使用。

（4）jQuery API中文手册：根据最新的 jQuery 1.11.x 和 2.1.x 版本翻译的 jQuery API 中文文档/手册。

（5）Headroom.js隐藏或展示页面元素：一个轻量级、纯 JavaScript 组件，用来隐藏或展现页面上的元素，为你的页面留下更多展示内容的空间。

（6）Responsive Nav响应式导航是一个很小的JS插件，压缩之后仅有1.7KB，能帮你创建针对小屏幕的可切换式导航。




Tips:在修改模板的过程中，锻炼了你查找东西的能力，根据功能找到对应的代码段，然后进行代码学习的能力，当然，还有PS的能力。

     
启动服务器的时候如果发现提示端口被占用，直接进cmd，输入命令netstat -ano，查看对应的TCP中哪个程序占用的，记住PID号，然后打开任务管理器，在查看里面调出PID，然后找到对应的进程，删掉就可以了。
