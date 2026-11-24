# Aaranya Cafe Website

A responsive single-page marketing site for Aaranya Cafe, built with plain HTML
and CSS — no build step and no JavaScript framework required.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Page markup: navbar, hero, marquee strip, story, CSS-only tabbed menu, features, gallery, offers, testimonials, visit/contact, footer |
| `style.css` | Full stylesheet with CSS variables, animations, reveal effects and responsive breakpoints |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is (no Jekyll processing) |
| `.github/workflows/deploy-pages.yml` | GitHub Actions workflow that mirrors the static files to the `gh-pages` branch |

Fonts come from Google Fonts and photos from the Unsplash CDN, so those need an
internet connection.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Imagery

The supplied design referenced an `assets/images/` folder that wasn't included.
All 27 image slots now use hotlinked, working Unsplash CDN photos with
`?auto=format&fit=crop&w=...&q=80` sizing. Replace any `src` URL with a local
path if you add your own photography later.

## Deployment

Live site: https://gowthamgaraga18-lab.github.io/CAFE-WEBSITE/

GitHub Pages is enabled and publishes from `main`, folder `/ (root)`. Merging the
working branch `arena/6601410d-cafe-website` into `main` publishes the site;
every later merge updates it automatically.

The workflow additionally mirrors the static files to `gh-pages` on each push to
the working branch, so Pages can alternatively be pointed at `gh-pages` / `(root)`
in **Repository Settings → Pages → Build and deployment**.

## Before going live

- The contact details in `index.html` are sample values (12 Heritage Lane, MG
  Road, Bengaluru 560001; +91 98765 43210; hello@aaranyacafe.in).
- The footer year is `2026`; bump it at the start of each new year.
- Social links in the footer are generic placeholders.
