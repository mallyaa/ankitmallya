# Jekyll site — deploy to GitHub Pages

Personal site with **Home** (photo + who I am), **Experience**, **Blog**, and **CV**.

## Deploy to mallyaa.github.io/mallyaa/

1. Copy this repo’s **root** contents (this folder) into the **root** of the **mallyaa** repo.
2. In the mallyaa repo, ensure `_config.yml` has `baseurl: "/mallyaa"`.
3. **Settings → Pages** → Deploy from branch **main** → Folder **/ (root)**.
4. Add your photo at `assets/img/photo.jpg`. Optional: add `assets/cv.pdf` for the CV Download button.

## Blog posts

Add files in `_posts/` named `YYYY-MM-DD-title.md` with front matter:

```yaml
---
layout: post
title: "Your title"
date: 2025-02-08
---
```

## Build locally

```bash
bundle install
bundle exec jekyll serve --baseurl ''
```

Open http://localhost:4000
