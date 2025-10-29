# Content Creation Guide

## Creating New Posts

To create a new journal entry or technical note, use Hugo's new content command:

```bash
hugo new posts/my-new-post.md
```

Or create the file manually in `content/posts/` directory.

## Post Structure

Each post should start with front matter (YAML format):

```markdown
---
title: "Your Post Title"
date: 2025-01-27
draft: false
description: "Brief description of the post"
tags: ["tag1", "tag2", "tag3"]
---

Your content here in Markdown...
```

## Post Fields

- **title**: The main heading of your post
- **date**: Publication date (format: YYYY-MM-DD)
- **draft**: Set to `true` to hide from site, `false` to publish
- **description**: Short description (used in meta tags and previews)
- **tags**: Array of tags for categorization

## Tips for Journaling

1. **Draft Mode**: Set `draft: true` while writing, then change to `false` when ready to publish
2. **Tags**: Use consistent tags like:
   - `journal` - Personal reflections
   - `tech` - Technical notes
   - `learning` - New things learned
   - `projects` - Project notes
   - `architecture` - System design thoughts
3. **Dates**: Use meaningful dates - you can backdate posts to reflect when you actually learned/wrote about something

## Preview Locally

Run the Hugo development server:

```bash
hugo server -D
```

The `-D` flag includes draft posts. Visit `http://localhost:1313` to see your site.

## File Organization

```
content/
  posts/
    welcome.md
    sample-tech-note.md
    your-new-post.md
```

All posts in `content/posts/` will automatically appear on your homepage below the profile section.

## Markdown Features

You can use all standard Markdown features:
- Headers (`#`, `##`, `###`)
- Lists (bullet and numbered)
- **Bold** and *italic* text
- `Inline code` and code blocks
- Links: `[text](url)`
- Images: `![alt](image.jpg)`

## Code Blocks

Use triple backticks for code blocks with syntax highlighting:

````markdown
```python
def hello():
    print("Hello, World!")
```
````

Languages supported: python, javascript, go, rust, java, and many more.

## Images

1. Place images in `static/images/` directory
2. Reference them in markdown: `![Description](/images/your-image.jpg)`
3. Or use relative paths for post-specific images in `content/posts/images/`

