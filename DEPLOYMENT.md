# Deployment & Contribution Guide

## Knowledge Base Structure

We use a strict **Category > Sub-category > Article** hierarchy.

## 1. Naming Conventions

### Directories
- **Format:** Lowercase, hyphen-separated (kebab-case). English only.
- **Examples:**
  - ✅ `artificial-intelligence`
  - ❌ `AI-ML`, `ArtificialIntelligence`

### Files
- **Format:** Lowercase, hyphen-separated. English only.
- **Examples:**
  - ✅ `small-vram-large-model-myth.md`
  - ❌ `Small VRAM Myth.md`

## 2. Taxonomy

Place new content in the most specific relevant folder under `content/knowledge/`.

| Category | Description | Sub-categories |
|----------|-------------|----------------|
| **technology** | Hard skills & engineering | `artificial-intelligence`, `software-engineering`, `infrastructure` |
| **business** | Commercial & Product | `product-management`, `startup-venture` |
| **industry** | Vertical market deep-dives | `semiconductor`, `automotive`, `healthcare` |
| **insights** | Soft skills & philosophy | `psychology`, `trends`, `philosophy` |
| **tools** | Hardware & Software reviews | `software`, `hardware` |
| **reading** | Reading notes | `books`, `articles`, `papers`, `cases` |

## 3. Creating a New Article

### Step 1: Choose Location
Identify the correct subdirectory based on the taxonomy above.

### Step 2: Create File
```bash
touch content/knowledge/technology/artificial-intelligence/my-new-topic.md
```

### Step 3: Add Frontmatter
Every file MUST start with:
```yaml
---
title: Your Title Here (Chinese OK)
date: YYYY-MM-DD
tags:
  - tag1
  - tag2
draft: false
---
```

### Step 4: Write Content
Use standard Markdown. You can use Chinese in the content.

## 4. Creating a New Category

If a topic doesn't fit existing folders:

1. **Create folder:**
   ```bash
   mkdir content/knowledge/technology/new-category-name
   ```

2. **Create index file:**
   ```bash
   touch content/knowledge/technology/new-category-name/index.md
   ```

3. **Add frontmatter to index:**
   ```yaml
   ---
   title: New Category Name
   description: Brief description
   ---
   
   # New Category Name
   
   Description of this category.
   
   ## Articles
   
   - [[article-slug|Article Title]]
   ```

## 5. Deployment

This site is built with **Quartz**.

### Local Preview
```bash
npx quartz build --serve
```

### Production Deployment
Changes pushed to the `main` branch are automatically deployed via GitHub Actions.

### Build Status
Check build status at: `https://github.com/YeYe-Kuris/daily-notes/actions`

## 6. Common Issues

### Emoji/Unicode in Titles
- Avoid emoji in file names and directory names
- Avoid Chinese punctuation in titles (use `?` not `？`)
- ✅ `title: "Hello World?"`
- ❌ `title: "Hello World？"`

### 404 Errors
If you get 404 after deployment:
1. Check the file exists in the correct location
2. Ensure the index.md file exists in parent directories
3. Check GitHub Actions build log for errors

## 7. File Organization Example

```
content/knowledge/
├── index.md                          # Knowledge base homepage
├── technology/
│   ├── index.md                      # Tech category page
│   ├── artificial-intelligence/
│   │   ├── index.md                  # AI sub-category page
│   │   └── small-vram-large-model-myth.md  # Article
│   └── software-engineering/
│       └── index.md
├── business/
│   ├── index.md
│   └── product-management/
│       └── index.md
└── ...
```

---

*Last Updated: 2026-02-04*
