---
title: "如何用 Hugo 搭建个人博客"
date: 2026-03-09T14:30:00+08:00
draft: false
tags: ["技术", "Hugo", "博客"]
categories: ["技术"]
---

Hugo 是一个用 Go 语言编写的静态网站生成器，以其极快的构建速度著称。

<!--more-->

## 为什么选择 Hugo

- **速度快**：每秒可以生成数千页面
- **主题丰富**：有大量精美的主题可选
- **单二进制文件**：单个可执行文件，无需依赖
- **Markdown 支持**：使用 Markdown 写作，简单高效

## 安装 Hugo

```bash
# macOS
brew install hugo

# Windows
choco install hugo-extended

# Linux
sudo apt install hugo
```

## 创建新站点

```bash
hugo new site myblog
cd myblog
git init
```

## 添加主题

```bash
git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
```

然后在 `hugo.toml` 中设置主题。

## 创建文章

```bash
hugo new content posts/hello.md
```

## 本地预览

```bash
hugo server -D
```

## 部署到 GitHub Pages

使用 GitHub Actions 自动部署，每次推送代码后自动构建发布。

---

Hugo 让搭建博客变得非常简单，推荐尝试！
