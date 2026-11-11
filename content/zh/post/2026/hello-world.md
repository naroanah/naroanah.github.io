+++
title = "开篇：用 Hugo 与 PaperMod 搭建个人博客"
date = 2026-11-11T16:30:00+08:00
lastmod = 2026-11-11T16:30:00+08:00
tags = ["hugo", "blog", "workflow"]
categories = ["技术笔记"]
draft = false
toc = true
showQuote = true
highlighted = true
+++

## <span class="section-num">1</span> 缘起 {#缘起}

持续写作是梳理知识与沉淀思考最有效的方式之一。这个博客基于 **Hugo** 静态站点生成器与 **PaperMod** 主题搭建，保留了极简的阅读排版与快速的构建体验。

## <span class="section-num">2</span> 核心特性 {#核心特性}

站点内置了日常技术写作所需的常用特性：

- **中英双语切换**：默认中文（`/zh/`），同时支持英文页面（`/en/`）。
- **霞鹜文楷排版**：正文采用 LXGW WenKai 字体，兼顾中文长文阅读体验与代码块等宽对齐。
- **归档写作热力图**：在「归档」页面基于 ECharts 自动统计每篇文章的字数与发布日期，并展示精选文章（`highlighted = true`）。
- **文首随机格言**：在 Front Matter 中开启 `showQuote = true` 即可在标题下方展示格言引用。

### <span class="section-num">2.1</span> 数学公式支持 {#数学公式支持}

内置 KaTeX 渲染，支持行内公式如 $E = mc^2$ 以及独立公式块：

$$
\mathcal{L}(\theta) = \mathbb{E}_{x \sim p_{\text{data}}} \left[ -\log p_{\theta}(x) \right]
$$

### <span class="section-num">2.2</span> 代码高亮与一键复制 {#代码高亮与一键复制}

```python
from dataclasses import dataclass

@dataclass
class Post:
    title: str
    tags: list[str]
    highlighted: bool = False

    def summary(self) -> str:
        return f"{self.title} ({', '.join(self.tags)})"
```

## <span class="section-num">3</span> 常用写作命令 {#常用写作命令}

在本地预览与新建文章：

```bash
# 启动本地实时预览（含草稿）
hugo server -D

# 新建一篇中文博文
hugo new content/zh/post/2026/my-new-post.md
```
