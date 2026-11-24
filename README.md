# Aaranya Cafe Website

A responsive single-page website for Aaranya Cafe, built with plain HTML and CSS (no build step required).

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Page markup: navigation, hero, story, menu, features, gallery, offers, testimonials, contact, footer |
| `style.css` | All styling, including responsive breakpoints at 1000px, 768px and 480px |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is (no Jekyll processing) |
| `.github/workflows/deploy-pages.yml` | GitHub Actions workflow that publishes the site to the `gh-pages` branch |

Images are loaded from Unsplash and fonts from Google Fonts, so an internet connection is needed for those assets.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Deployment

This site is published with **GitHub Pages** at:

https://gowthamgaraga18-lab.github.io/CAFE-WEBSITE/

On every push to `arena/6601410d-cafe-website`, the `deploy-pages.yml` workflow
copies the static files into the `gh-pages` branch, which is the Pages publishing
source. Creating that branch is also what enables Pages for the repository
(GitHub does this automatically, no settings change needed).

Each push to the working branch re-runs the deployment. If the site ever needs
to be published from `main` instead, change the Pages source in
**Repository Settings → Pages → Build and deployment** and update the workflow's
`branches` filter.

## Before going live

Replace the placeholder details in `index.html`:

- Cafe address in the contact section
- Phone number (`+91 XXXXX XXXXX`) and the `tel:` link
- Social media links in the footer
