---
title: 使用 Hexo 创建博客并使用 GitHub Pages 和 Cloudflare 实现自定义域名以及 HTTPS
date: 2022-04-18 22:22:22
tags: Hexo, GitHub Pages, Cloudflare, HTTPS, Blog
---

# 什么是 Hexo

Hexo 是一个使用 Markdown 编写文章并生成静态网页的博客系统。

# 安装 Hexo

以下都是基于 WSL1 Ubuntu 的操作。

官方安装文档：
https://hexo.io/zh-cn/docs/


## 安装依赖

* Node.js 10.13+
* Git

```shell
# 安装 nodejs
# https://github.com/nodesource/distributions/blob/master/README.md#debinstall
curl -fsSL https://deb.nodesource.com/setup_17.x | sudo -E bash -
sudo apt update
sudo apt install -y nodejs

# 安装 git
sudo apt install -y git
```

## 安装 Hexo

```shell
sudo npm install -g hexo-cli
```

# 创建博客

官方文档：
https://hexo.io/zh-cn/docs/setup

```shell
# 创建博客
hexo init blog
cd blog
npm install
# 启动博客内置的服务器
hexo server
```

通过浏览器访问 `http://localhost:4000/` 博客

# 配置博客

官方文档：
https://hexo.io/zh-cn/docs/configuration

# 新建文章

官方文档：
https://hexo.io/zh-cn/docs/writing

```shell
hexo new <blog-name>
```

# 生成静态页

```shell
hexo generate
```

# 创建 Github Page 项目

官方文档：
https://hexo.io/zh-cn/docs/github-pages

项目名为：<你的 GitHub 用户名>.github.io



# 配置发布

