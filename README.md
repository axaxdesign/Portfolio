# Axel Bäckström — portfolio

Static site. No build step: every page is plain HTML that loads `support.js` locally and React from a CDN.

## Structure

- `index.html` — routes by screen width: phones to `home-mobile.html`, everything else to `home.html`
- `work.html`, `about.html`, `project-001.html` … `project-006.html` — desktop pages
- `*-mobile.html` — the mobile counterparts
- `assets/` — photographs, films, logo
- `support.js` — page runtime

## Publish with GitHub Pages

1. Create an empty repository on GitHub.
2. From this folder:

   git init
   git add .
   git commit -m "Portfolio"
   git branch -M main
   git remote add origin https://github.com/USERNAME/REPO.git
   git push -u origin main

3. Repository → Settings → Pages → Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.

The site appears at `https://USERNAME.github.io/REPO/`.

## Note

The three bås films total about 13 MB and load with the page. Compress them before publishing if mobile data matters. GitHub blocks single files over 100 MB.
