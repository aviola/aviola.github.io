# aviola.github.io

Personal blog built with [Hugo](https://gohugo.io) and the
[PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme (added as a
git submodule under `themes/PaperMod`).

## Writing a post

Add a Markdown file under `content/posts/`, e.g. `content/posts/my-post.md`:

```md
---
title: "My Post"
date: 2026-09-04
tags: ["some-tag"]
---

Post content here.
```

That's it — no build step, no components.

## Running locally

```sh
git clone --recurse-submodules https://github.com/aviola/aviola.github.io.git
cd aviola.github.io
hugo server -D
```

If you already cloned without `--recurse-submodules`, run:

```sh
git submodule update --init --recursive
```

## Deploying

Pushing to `main` triggers `.github/workflows/deploy.yml`, which builds the
site with Hugo and publishes it to GitHub Pages.

## TODO before going live

- [ ] Replace `static/images/avatar.jpg` with a real photo
- [ ] Set your real bio/subtitle and social links in `hugo.yaml` (`params.profileMode`, `params.socialIcons`)
