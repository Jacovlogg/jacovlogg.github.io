# Build & Break

A personal blog about software architecture, systems design, and evolving ideas.
Built with [Jekyll](https://jekyllrb.com/) and the [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) theme,
deployed automatically to [GitHub Pages](https://pages.github.com/).

🌐 **Live site:** <https://jacovlogg.github.io>

---

## Running locally

**Prerequisites:** [Docker Desktop](https://www.docker.com/products/docker-desktop/)

```bash
docker compose up
```

Then open <http://localhost:4000> in your browser.
The site live-reloads automatically when you save a file.

> First run will take a minute to pull the image and install gems.
> Subsequent runs are fast thanks to the cached gem volume.

---

## Writing a new post

Create a file in `_posts/` following the naming convention:

```
_posts/YYYY-MM-DD-your-post-title.md
```

Minimal front matter:

```yaml
---
title: "Your Post Title"
date: 2026-01-01 12:00:00 +0200
categories: [category]
tags: [tag1, tag2]
---

Post content here.
```

---

## Deployment

Pushing to `main` automatically triggers the GitHub Actions workflow
(`.github/workflows/pages-deploy.yml`), which builds the site with Jekyll and
deploys it to GitHub Pages. No manual steps needed.
