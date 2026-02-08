# Jekyll one-stop site for GitHub Pages

Personal site with **Home** (photo + who I am), **Experience**, **Blog**, and **CV**. Built with Jekyll so GitHub Pages builds it automatically.

## What’s included

| Page       | Purpose |
|-----------|---------|
| **Home**  | Display photo, name, tagline, short “who I am” snippet, quick links |
| **Experience** | Work highlights, what you bring, where you’re headed |
| **Blog**  | List of posts; add files in `_posts/` (e.g. `2025-02-08-title.md`) |
| **CV**    | CV page + “Download PDF” and “LinkedIn” buttons |

## Deploy as your GitHub.io page

1. **Copy this folder’s contents** into the **root** of the repo that serves your site:
   - For **username.github.io** → repo name is `username.github.io` (e.g. `mallyaa.github.io`).
   - For **username.github.io/repo-name/** → repo name is `repo-name` (e.g. `mallyaa`).

2. **Set `baseurl` in `_config.yml`:**
   - If the site is at **https://mallyaa.github.io** (user site): use `baseurl: ""`.
   - If the site is at **https://mallyaa.github.io/mallyaa/** (project site): use `baseurl: "/mallyaa"`.

3. **Add your photo:** Put a square headshot at **`assets/img/photo.jpg`**.  
   If it’s missing, the site shows an “AM” placeholder.

4. **Optional — CV PDF:** Put your CV at **`assets/cv.pdf`**. The CV page “Download PDF” button will link to it.  
   If you don’t add a PDF, edit `cv.md` and remove or change that button.

5. **Turn on GitHub Pages:** Repo **Settings → Pages** → Source: **Deploy from a branch** → Branch: **main** (or your default) → Folder: **/ (root)** → Save.  
   GitHub will build the Jekyll site and serve it.

## Writing blog posts

Create a file in **`_posts/`** with the name:

```text
YYYY-MM-DD-your-title.md
```

Example: `2025-02-08-first-post.md`. At the top add:

```yaml
---
layout: post
title: "Your post title"
date: 2025-02-08
---
```

Then write your post in Markdown below the `---`. It will appear on the Blog page and get its own URL.

## Build locally (optional)

```bash
cd jekyll-site   # or the root of the repo you copied into
bundle install
bundle exec jekyll serve
```

Open http://localhost:4000 (and add `--baseurl ''` or your baseurl if needed).
