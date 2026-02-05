# KB Restructure - File Generation Task

## Task
Generate complete file contents for knowledge base restructure.

## Required Files

### 1. content/knowledge/index.md
Main knowledge base homepage with:
- Links to all 6 categories
- Latest articles table (1 article exists)
- Status badges (1 article vs under construction)

### 2. content/knowledge/technology/index.md  
Technology category page with links to:
- artificial-intelligence/ (has 1 article)
- software-engineering/ (empty)
- infrastructure/ (empty)

### 3. content/knowledge/technology/artificial-intelligence/index.md
AI subcategory with article list:
- small-vram-large-model-myth.md

### 4. content/knowledge/technology/software-engineering/index.md
Empty category placeholder

### 5. content/knowledge/technology/infrastructure/index.md
Empty category placeholder

### 6. content/knowledge/business/index.md
Business category with links to:
- product-management/ (empty)
- startup-venture/ (empty)

### 7. content/knowledge/industry/index.md
Industry category (empty)

### 8. content/knowledge/insights/index.md
Insights category (empty)

### 9. content/knowledge/reading/index.md
Reading category (empty)

### 10. content/knowledge/tools/index.md
Tools category (empty)

### 11. content/knowledge/business/product-management/index.md
Empty subcategory

### 12. content/knowledge/business/startup-venture/index.md
Empty subcategory

## Output Format
For each file, output:
```
=== FILE: path/to/file ===
[complete file content]
=== END ===
```

Requirements:
- Use English for directory/file names
- Chinese OK for titles and content
- Include proper frontmatter
- Include navigation links
