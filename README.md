# Maple Structural Engineering — Website

Single-page static website for **Maple Structural Engineering**, hosted via GitHub Pages at
[hamidrezarashidi.github.io](https://hamidrezarashidi.github.io).

## Stack

- Plain HTML + CSS + a few lines of JS — no build step required
- Inter + Fraunces from Google Fonts
- Inline SVGs for every figure so the site stays fast and crisp on retina displays
- `.nojekyll` disables GitHub's default Jekyll build so files under `assets/` are served as-is

## Structure

```
.
??? index.html          # Page markup
??? styles.css          # All styling (maple red + white palette)
??? script.js           # Sticky nav + reveal-on-scroll
??? assets/             # Logo, icons, figures, project placeholders
??? .nojekyll
??? README.md
```

## Local preview

Because everything is static, you can open `index.html` directly or run any local web server:

```bash
python3 -m http.server 4000
# then open http://localhost:4000
```

## What to customize next

- `index.html` — copy in every section (hero, services, process, projects, FAQ, CTA)
- `assets/project-*.svg` — replace with real project photos (drop in PNG/JPG and update the `src`)
- Contact links — replace the placeholder email (`hello@maplestructural.com`) and phone number
- Colors — the single source of truth is the `:root` block at the top of `styles.css`
  - `--maple`: primary red (`#C8102E`)
  - `--maple-dark`: hover red
  - `--maple-soft`: tinted backgrounds
