---
title: 从零部署Hexo
date: 2024-12-29 18:49:10
tags: hexo,github 
---


# Hexo 部署
## 一、Hexo概念：
### 适合入门的一个简单快效的博客框架

## 二、安装
### 要求:
先安装好Git和Node.js(Node.js 版本需不低于 10.13，建议使用 Node.js 12.0 及以上版本)

### 安装Hexo
所有必备的应用程序安装完成后，即可使用npm安装 Hexo。
1. 命令：`npm install -g hexo-cli`  
![运行结果](/images/first/g.png)

2. 命令：`hexo init 文件夹名`（如blogt）  
![创建文件夹](/images/first/folder.png)

3. 命令：`cd 文件夹名 ` + `npm install`  
![npm](/images/first/npminstal.png)

### 配置
在 _config.yml或代替配置文件中修改大部分的配置。

1. 打开blogtwo下的_config.yml配置文件。  
![config](/images/first/config.png)

2. 在配置文件中设置网站信息（Site部分）。  
![title](/images/first/title.png)

3. 在配置文件中设置网址信息（URL部分）。  
![web](/images/first/web.png)

4. 注意：theme是你所引用的主题的名称  
![theme](/images/first/theme.png)

### 安装主题
安装并配置好Hexo后，在同文件夹下，安装所需要的主题即可。  
1. 命令： `cd themes`+ `git clone https://github.com/theme-particlex/hexo-theme-particlex.git particlex --depth=1`  
![cdthemes](/images/first/cdthemes.png)

2. 启动查看命令： `hexo server`
![server](/images/first/server.png)

## 三、参考文献
1. 参考链接：https://hexo.io/zh-cn/docs/
2. 参考链接：https://github.com/theme-particlex/hexo-theme-particlex