# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal portfolio and blog site built with Jekyll (GitHub Pages). The site uses the `jekyll-theme-minimal` theme and is deployed to azharkhalid.com.

## Key Commands

### Local Development
```bash
# Install Bundler (if not already installed)
gem install bundler

# Install Jekyll and dependencies
bundle install

# Serve locally at http://localhost:4000
bundle exec jekyll serve
```

### Build
```bash
# Build the site for production
bundle exec jekyll build
```

## Architecture

### Site Structure
- `_config.yaml` - Jekyll configuration (theme, permalinks, defaults)
- `_layouts/` - Custom layouts (post.html for blog posts)
- `_posts/` - Blog posts in Jekyll format: `YYYY-MM-DD-title.md`
- `images/` - Static image assets
- `index.md` - Homepage (portfolio/resume)
- `blog.md` - Blog index page that lists all posts

### Blog Post Format
Posts in `_posts/` require Jekyll front matter with title and date:
```yaml
---
title: Post Title Here
date: 2026-01-30 00:00:00 +0700
---
```

The `date` field should use `+0700` timezone (WIB/Indonesia).

### Layout System
- All posts use `layout: post` (automatically applied via `_config.yaml` defaults)
- Custom layout: `_layouts/post.html` displays post title, date, and content
- Pages use `layout: default` (from jekyll-theme-minimal theme)

### Permalinks
Blog posts follow the pattern: `/blog/:year/:month/:day/:title/`

This is configured in `_config.yaml` and generates URLs like `/blog/2026/01/30/my-post-title/`.

## Deployment

This is a GitHub Pages repository:
- Source files are pushed to the `master` branch
- GitHub automatically builds and deploys via Jekyll
- Custom domain configured via CNAME file
