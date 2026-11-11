# Aoran Han's Blog (`naroanah.github.io`)

基于 [Hugo](https://gohugo.io/) 与 [PaperMod](https://github.com/adityatelange/hugo-PaperMod) 构建的中英双语个人博客，参考并定制自 [ramsayleung/ramsayleung.github.io](https://github.com/ramsayleung/ramsayleung.github.io)。

## 目录结构

- `config.yml`：站点核心配置（个人信息、导航菜单、多语言、Giscus 评论、社交图标）
- `content/zh/`：中文内容目录（默认语言）
  - `content/zh/post/`：中文博客文章
  - `content/zh/about.md`：中文关于页面
  - `content/zh/archives.md`：中文归档页（含写作热力图与精选阅读）
  - `content/zh/search.md`：中文搜索页
- `content/en/`：英文内容目录
  - `content/en/post/`：英文博客文章
  - `content/en/about.md`：英文关于页面
- `data/quotes.yaml`：文首随机格言词库（文章开启 `showQuote = true` 时生效）
- `layouts/`：定制模板（ECharts 归档写作热力图、KaTeX 公式、图片点击放大、下拉导航栏）
- `assets/css/extended/`：扩展样式（霞鹜文楷字体、代码块样式、归档卡片与图片缩放）

## 本地预览与写作

```bash
# 本地启动开发服务器（默认 http://localhost:1313）
hugo server -D

# 新建中文文章
hugo new content/zh/post/2026/your-post-name.md

# 构建静态文件到 ./public
hugo --minify
```

## 文章 Front Matter 常用字段

```toml
+++
title = "文章标题"
date = 2026-11-11T16:30:00+08:00
lastmod = 2026-11-11T16:30:00+08:00
tags = ["tag1", "tag2"]
categories = ["技术笔记"]
draft = false
toc = true
showQuote = true      # 是否在标题下展示随机格言
highlighted = true    # 是否展示在归档页「精选阅读」中
+++
```
