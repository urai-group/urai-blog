---
title: "Welcome"
date: 2025-11-27T12:00:00Z
draft: false
authors:
  - "URAI"
summary: "Welcome to the URAI blog website"
weight: 1
---

## Introduction

This guide covers the essential steps and advanced features—including LaTeX, figures, and custom HTML/CSS—for publishing research blogs on your Hugo site.

## 1. Creating a New Blog Post

All blog posts are written in Markdown format and stored as files.

### 📝 Step 1: Generate the Post File

Use the following command in your site's root directory to create a new file. This command automatically sets up the necessary structure.

```bash
hugo new posts/your-post-title.md
```

**Tip:** Use lowercase and hyphens (e.g., `ai-in-biology` not `AI in Biology`).

### ⚙️ Step 2: Edit the Front Matter

Open the newly created Markdown file (`content/posts/your-post-title.md`). The section at the top enclosed by `---` is the **Front Matter**:

| Field | Description | Example |
| :--- | :--- | :--- |
| `title` | The main title of your post | `"A Deep Dive into Transformer Architectures"` |
| `date` | The publication date | `2025-11-28T10:00:00+01:00` |
| `author` | The author(s) name | `"Dr. Anya Schmidt"` |
| `draft` | Set to `true` while working, `false` to publish | `false` |
| `tags` | Keywords for categorization | `["AI", "Deep Learning", "NLP"]` |

## 2. Writing Content with Scientific Formatting

### 📜 Markdown Basics

| Feature | Markdown Syntax |
| :--- | :--- |
| **Heading 2** | `## Your Sub-Section Title` |
| *Italics* | `*text*` or `_text_` |
| **Bold** | `**text**` or `__text__` |
| Lists | `* Item 1` or `1. Item 1` |
| Code Blocks | ` ```python\nprint("Hello")\n``` ` |
| Blockquotes | `> This is a cited quote.` |

### 📐 LaTeX for Equations (MathJax)

**Inline Equations:** Use single dollar signs: `$E=mc^2$` → $E=mc^2$

**Display Equations:** Use double dollar signs:
```latex
$$
\nabla \cdot \mathbf{E} = \frac{\rho}{\varepsilon_0}
$$
```

### 🖼️ Including Figures and Images

1. **Create a Page Bundle:** Rename your post file to `index.md` inside a folder named `your-post-title/`
2. **Add Images:** Place images directly into this folder
3. **Embed in Post:** `![A caption describing the image](model-architecture.png)`

**Tip:** Use high-resolution images and SVG for diagrams.

## 3. Advanced Features

### 🎨 CSS-Embedded HTML

```html
<figure style="text-align: center;">
  <img src="your-plot.png" alt="A plot showing loss over epochs">
  <figcaption style="font-style: italic; color: #555;">
    Figure 1: Loss function convergence for the ResNet model.
  </figcaption>
</figure>
```

### 📹 Embedding YouTube Videos

`{{< youtube YOUTUBE_VIDEO_ID >}}`

### 🔗 Citations and References

```markdown
## References

1. A. Schmidt, et al. "Transformer-based Model for Text Classification." *Journal of AI Research*, 2024.
2. I. Goodfellow, et al. *Deep Learning*. MIT Press, 2016.
```

## 4. Publishing Your Post

### 💻 Local Preview

```bash
hugo server -D
```

Visit `http://localhost:1313/` to verify formatting, LaTeX, and images.

### 🚀 Deployment

1. Set `draft: false` in Front Matter
2. Build the site: `hugo`
3. Sync the `/public` directory to your hosting server

