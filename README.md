# dk-clouddusk blog

This repo is a simple static blog for Azure, Microsoft Fabric, and cloud networking notes.

## How to add a new post

1. Create a new HTML file under the `posts/` folder.
2. Use the same page structure as the existing article in `posts/2026-08-15-fabric-private-link.html`.
3. Add a new card to the homepage in `index.html` linking to the new article.
4. Commit and push to GitHub.

## Publishing

The repo is already configured for GitHub Pages via `.github/workflows/static.yml`.

## Weekly workflow

A simple weekly pattern is:

- write the article
- save under `posts/`
- add it to the homepage
- commit and push

This keeps the blog lightweight and easy to maintain without a heavy CMS.
