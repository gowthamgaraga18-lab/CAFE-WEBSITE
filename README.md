# Aaranya Cafe Website

A responsive single-page website for Aaranya Cafe, built with plain HTML and CSS (no build step required).

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Page markup: navigation, hero, story, menu, features, gallery, offers, testimonials, contact, footer |
| `style.css` | All styling, including responsive breakpoints at 1000px, 768px and 480px |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is (no Jekyll processing) |

Images are loaded from Unsplash and fonts from Google Fonts, so an internet connection is needed for those assets.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Deployment

This site is published with **GitHub Pages** from the repository root of the
`arena/6601410d-cafe-website` branch.

Live URL: https://gowthamgaraga18-lab.github.io/CAFE-WEBSITE/

Every push to that branch triggers a new Pages build. To publish from `main`
instead, change the Pages source branch in
**Repository Settings → Pages → Build and deployment**.

## Before going live

Replace the placeholder details in `index.html`:

- Cafe address in the contact section
- Phone number (`+91 XXXXX XXXXX`) and the `tel:` link
- Social media links in the footer
