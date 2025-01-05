---
title: 在GitHub上部署Hexo
date: 2025-1-5 15:35:10
tags: hexo,github pages
---

使用GitHub pages部署静态博客的教程。
<!-- more -->

# 在GitHub上部署Hexo
#### 此方法适用于公开或私人储存库. 若你不希望将源文件夹上传到 GitHub，请参阅其他相关方法。

## 一、Git概念
#### 是一个开源的分布式版本控制系统，一般用于合作项目管理。

## 二、创建GitHub存储库
若之前已将 Hexo 上传至其他储存库，将该储存库重命名即可。

### 创建
在https://github.com/上操作

1. 建立一个名为 "xxx.github.io" 的repository存储库（如username.github.io ）  
![createrstry](/images/two-creategithub/createrstry.png)

2. 查看存储库是否创建成功  
![checkrstry](/images/two-creategithub/checkrstry.png)

### 部署
将创建好的资源库克隆到本地，并进行修改上传

1. 将GitHub资源库拉到本机`git clone https://github.com/username/username.github.io`
![gitclone](/images/two-creategithub/gitclone.png)  

2. 将main分支上传到GitHub上`git push -u origin main`  
     若未更新内容上传，终端则会显示：  
     ![emptygitpush](/images/two-creategithub/emptygitpush.png)   
     若更新了内容上传，终端则会显示：  
     ![fullgitpush](/images/two-creategithub/fullgitpush.png)  

3. 在GitHub储存库中前往 Settings > Pages > Source,将source改成 GitHub actions  
![deploymentactions](/images/two-creategithub/deploymentactions.png)  

4. 在储存库中创建ages.yml文件，文件路径:".github/workflows/pages"  
![createpages](images/two-creategithub/createpages.png)  


### 配置
将GitHub上的pages版本更改为电脑上安装的版本型号  

1. 获取本地node版本信息  
![nodeversion](/images/two-creategithub/nodeversion.png)  
 
2. 更改pages.yml文件中的node-version  
![modifypages](/images/two-creategithub/modifypages.png)  

## 三、参考文献
参考链接：https://hexo.io/zh-cn/docs/github-pages.html  



