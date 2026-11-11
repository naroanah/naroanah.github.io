+++
title = "Hello World: Building My Blog with Hugo and PaperMod"
date = 2026-11-11T16:30:00+08:00
lastmod = 2026-11-11T16:30:00+08:00
tags = ["hugo", "blog", "workflow"]
categories = ["Tech Notes"]
draft = false
toc = true
showQuote = true
highlighted = true
+++

## <span class="section-num">1</span> Why Write {#why-write}

Writing is one of the best ways to clarify thoughts and document engineering journeys. This site is powered by **Hugo** and the **PaperMod** theme, designed for fast static generation and clean typography.

## <span class="section-num">2</span> Features {#features}

- **Bilingual Support**: Seamless switching between Chinese (`/zh/`) and English (`/en/`).
- **Activity Heatmap**: ECharts-powered contribution calendar on the Archives page, plus highlighted posts (`highlighted = true`).
- **KaTeX Math**: Inline math like $\nabla_{\theta} J(\theta)$ and display equations:

$$
\text{Attention}(Q, K, V) = \text{softmax}\left(\frac{QK^T}{\sqrt{d_k}}\right)V
$$

- **Syntax Highlighting**:

```rust
fn main() {
    println!("Hello, naroanah.github.io!");
}
```
