# adm-2k.github.io

Personal site of Aaron McKeever — [adm-2k.github.io](https://adm-2k.github.io).

A hand-rolled Jekyll theme on GitHub Pages. No JavaScript, no build pipeline
beyond what Pages runs automatically. Push to `main` and it deploys.

## Writing a post

Add one Markdown file to `_posts/`, named `YYYY-MM-DD-slug.md`:

```markdown
---
title: "Post title"
date: 2026-08-10
tags:
  - civic-tech
---

Body in plain Markdown.
```

Push, and it appears at `/writing/<year>/<slug>/`, on the
[writing page](https://adm-2k.github.io/writing/), on the home page's
recent-posts list, and in the RSS feed (`/feed.xml`). Nothing else to update.

## Editing the rest

| What | Where |
|------|-------|
| Home page hero, "Now" items, selected-work cards | Front matter in `index.md` |
| Full work record | `_pages/work.md` |
| About, résumé, writing index | `_pages/*.md` |
| Layouts (HTML shell) | `_layouts/` |
| Design system (colors, type, cards) | `assets/css/main.scss` |
| Résumé PDF | Replace `assets/Aaron_McKeever_Resume_Technical.pdf` |

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.
