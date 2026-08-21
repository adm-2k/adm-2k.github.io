# adm-2k.github.io

Personal site of Aaron McKeever — [adm-2k.github.io](https://adm-2k.github.io).

A hand-rolled Jekyll theme on GitHub Pages. No frameworks — one small
vanilla-JS file (`assets/js/main.js`) for the theme toggle and motion, and
the site works fully without it. Push to `main` and the
[Deploy site](.github/workflows/deploy.yml) workflow builds and publishes it
to the `gh-pages` branch; every pull request gets a live preview at
`/pr-preview/pr-<number>/` via
[PR preview](.github/workflows/pr-preview.yml).

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
| Home page hero, epigraph, "Currently" items, index entries | Front matter in `index.md` |
| Full work record | `_pages/work.md` |
| About, résumé, writing index | `_pages/*.md` |
| Layouts (HTML shell) | `_layouts/` |
| Design system (colors, type, cards) | `assets/css/main.scss` |
| Résumé PDF | Replace `assets/Aaron_McKeever_Resume.pdf` |

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.
