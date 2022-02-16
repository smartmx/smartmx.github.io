---
title: GithubPageCfg
description: How to Config GithubPage Settings.
---

### 前言

在其他博客网站上写博客都显得略微麻烦，markdown格式编写博客会变得十分简单。  
标准模板的Github Pages，只要上传markdown，就会自动生成html。  
并且现在Github同步十分容易，也免费，安全性有保障。  

### 开启Github Pages

首先要创建一个名字为 用户名.github.io 的仓库  
在仓库的setting/optional网页中可以找到GitHub Pages  
打开GitHub Pages，并去选择一个主题，本博客使用的是Cayman  

### 配置域名和https访问

Github Pages自带https加密功能，不需要用户自己准备。

### 索引markdown文件

在生成的网站中跳转到另一个markdown文件生成的网站，需要额外的配置：  
更改仓库中的__config.yml，添加如下代码：

```javascript
plugins:
  - jekyll-relative-links
relative_links:
  enabled: true
  collections: true
```

### 下面是访问测试

1.[test测试页面](githubpagetest.md)  

2.[dir test文件夹测试页面](githubpagetestfolder/githubpagefoldertest.md)

### 修改Hexo每个网页的标题和描述

在网页对应的markdown文件中，通过在文件头部添加以下代码：

```text
---
title: Your Title
description: Your description
---
```

## [博客主页](https://blog.maxiang.vip/)
