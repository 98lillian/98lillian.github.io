---
title: 在部署好的GitHub上面发布文章
date: 2025-1-6 14:50:10
tags: github pages，blog
---

如何在部署好的GitHub上面发布文章。
<!-- more -->

# 在GitHub上面发布文章
#### 该方法适用于用Visual Studio Code来编辑markdown文件，从而发布自己的个人github.io静态博客。若有其他需求，请参阅其他相关方法。

## 一、前期准备
#### 安装好Visual Studio Code软件，并了解一些markdown的知识。

## 二、获取GitHub存储库
若已经将GitHub文件拉到本地的话，可以跳过。

### 克隆到本机
在https://github.com/上与powershell操作   

1. 将GitHub上的网址复制下来  
![githubhttp](/images/three-acticle/githubhttp.png)  

2. 克隆到本机 `git clone https://github.com/XXX/XXX.github.io.git`  
![gitclone](/images/three-acticle/gitclone.png)  

### 创建文章
本地文件夹路径：./XXX.github.io > source > _posts/images  

1. 按照路径，找到_posts文件夹，在里面建立自己所需要编写上传的md文章(如three.md)  
![posts](/images/three-acticle/posts.png)  

2. 若涉及到需要上传图片，则要在与_posts同目录下创建一个存放图片的文件夹（如images）  
![images](/images/three-acticle/images.png) 

### 编写文章  
在vs code中打开md文件，并进行文章编写
![modifyaticle](/images/three-acticle/modifyaticle.png)  

### 上传文章
在vs code上传后，可以到GitHub上查看上传状态  

1. 将编辑好的文件上传至GitHub(如three.md)  
![commit](/images/three-acticle/commit.png)  
![sync](/images/three-acticle/sync.png)   

2. 上传后，在GitHub中的Action模块中，便可以看到上传进度了。  
注：黄色圆点表示正在运行，红色叉叉表示失败，绿色勾勾便是已经完成 
![actions](/images/three-acticle/actions.png)  

### 查看文章
上传成功后，便可以在https://XXX.github.io/网页上面看到该文章啦  
![article](/images/three-acticle/article.png)


