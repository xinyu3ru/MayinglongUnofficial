# 马应龙非官方网站Github仓库

---start---
## 目录(2021年05月25日更新)
---end---



## 用Github Actions写Markdown文章，自动更新到WordPress



- 写博客最舒服的格式是Markdown；

- 管理博客站最省心的方式是WordPress；

- 推广博客站最好的平台是Github；



这个项目可以让你用Markdown写博客，push更新到Github后，Github Actions自动将文章更新到WordPress，并将WordPres站的文章索引更新到Github仓库的README.md，供搜索引擎收录。



程序采用

[https://github.com/zhaoolee/WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools)






### 如何保护自己的WordPress账户密码？


Github 有一个secrets 功能，可以将用户名密码等关键信息保护起来，只有Github Actions可以读取到关键信息。

本项目需要设置三个secret



- WordPress登录用户名, 变量名为 USERNAME
- WordPress登录密码，变量名为 PASSWORD
- WordPress的xmlrpc.php，变量名为 XMLRPC_PHP








### 如何新建文章？

在`_post` 目录下新建 后缀为 `.md` 的markdown文件即可





### 文章管理：如何为文章分类/加关键词标签？

在 `.md` 文件顶部填写以下初始化信息，即可完成标题（title），标签（tags），分类（categories）的设置，**其中title为必填项目**








```
---
title: 我是标题
tags: 
- 我是0号标签关键词
- 我是1号标签关键词
- 我是2号标签关键词
categories:
- 我是1号分类
- 我是2号分类
---

```







## 标签(tags)和分类(categories)有什么区别？

标签(tags)是针对单篇文章的关键词，比如香蕉的标签有 **黄色**，**味甜** （标签是香蕉的属性）
分类(categories)是本篇文章的归属，比如香蕉的分类为 **水果**，**植物** 



###  如何设置固定链接？

对于博客而言，文章拥有一个固定的链接，是很重要的，我经过各种尝试，最终借鉴了 [简书](jianshu.com) 的文章url形式，域名后加 `/p/` , 再加英文文件名，只要不改变英文文件名，文章就有固定的链接，我在`_posts` 目录下新建一个 `2020-01-18-blog.md` 文件，同步后的文章url为 





文件名与网站url严格对应，既方便了修改，又可以在网站数据库出事故后，迅速从github仓库迅速恢复文章内容（容灾），连url都不会变。









### 程序永久开源更新地址(求Star):



[https://github.com/zhaoolee/WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools)



当我们把毕生所学，通过几十年如一日的博客更新，逐步开源到互联网上时，必将会造福更多志同道合的人。

