# Blog Workflow

## Local development

```bash
npm install
npm run server
```

Visit `http://localhost:4000`.

## Release check

```bash
npm run check
```

This rebuilds the site locally and catches most configuration or content errors before push.

## Publish a new post

1. Create a post: `npx hexo new post "Post Title"`
2. Write the post in `source/_posts/`
3. Put post images in the generated asset folder when needed
4. Run `npm run check`
5. Commit and push to `main`
6. Wait for the GitHub Pages workflow to turn green
7. Verify `https://cypher912.github.io`

## Recommended front matter

```yaml
---
title: Post Title
date: 2026-03-20 20:40:00
tags:
  - Hexo
categories:
  - Notes
description: Short summary for cards and search results.
cover:
---
```
