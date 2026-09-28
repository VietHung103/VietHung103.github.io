# VietHung103.github.io

Source for my personal site, built with Jekyll on a customized version of the
[texture](https://github.com/samarsault/texture-jekyll) theme. Strict black &
white theme, showing an About/Skills/Projects/Timeline/Contact page for
recruiters, professors, and collaborators.

## Local development

```
bundle install
bundle exec jekyll serve
```

## How to update content

**Add a timeline entry** (education, milestones, updates) — create a new file
in `_posts/` named `YYYY-MM-DD-slug.markdown` with front matter:

```yaml
---
layout: post
title:  "Entry title"
description: One-line summary (optional).
period:   "2023 - 2026"       # optional, shown on the entry's own page
categories: SomeTag            # optional
date: 2026-01-01
---

Body content in Markdown.
```

**Add a skill** — edit `_data/skills.yml`, adding an item to an existing
`category` group or a new group.

**Add a project** — edit `_data/projects.yml`, copying the existing entry's
shape (`name`, `description`, `role`, `date`, `tags`, optional `link`).

**Update identity/photo/bio** — edit the `texture:` block in `_config.yml`:
`title`, `tagline`, `bio`, `photo` (path to an image under `assets/`, e.g.
`assets/img/profile.jpg`), `social_links`, and the top-level `email`.

## License

The underlying theme is available as open source under the terms of the
[MIT License](https://opensource.org/licenses/MIT).
