# Dmitry Gofman — Personal Brand Landing Page

**Live preview:** [dima-builder.preview.emergentagent.com](https://dima-builder.preview.emergentagent.com)

A single static HTML file. No build step. No backend. Drop into any GitHub Pages branch.

---

## What's in this folder

- `/app/site/index.html` — the **deliverable**. Single self-contained file (HTML + CSS + JS embedded). Open it directly in a browser, or push it to GitHub Pages.

---

## Deploy to GitHub Pages (your existing repo)

Your existing site lives at: `https://github.com/dmitrygofman/homepage`

### Option A — replace the `main` branch root
```bash
# from your local clone of dmitrygofman/homepage
cp /path/to/site/index.html ./index.html
git add index.html
git commit -m "Rebuild personal brand landing page"
git push origin main
```
Then in your repo: **Settings → Pages → Source = `main` branch, `/ (root)`**.

### Option B — `gh-pages` branch
```bash
git checkout -b gh-pages
cp /path/to/site/index.html ./index.html
git add index.html
git commit -m "Deploy landing page"
git push origin gh-pages
```
Then: **Settings → Pages → Source = `gh-pages` branch, `/ (root)`**.

---

## Editing

Everything (HTML, CSS, JS) lives inside `index.html`. Open it in any editor.

### Common edits

| What | Where (search inside `index.html`) |
|---|---|
| Hero headline | `data-testid="hero-headline"` |
| Hero subheadline | `data-testid="hero-subheadline"` |
| Email | `mailto:dimagofman22@gmail.com` |
| LinkedIn | `linkedin.com/in/dima-gofman-52134a181` |
| GitHub | `github.com/dmitrygofman` |
| Color tokens | inside `<style>` → `:root { --copper: ...; }` |
| Fonts | Google Fonts `<link>` near top of `<head>` |

### Add a portrait
When you have a photo, drop it next to `index.html` (e.g. `portrait.jpg`) and add inside the hero section:
```html
<img src="portrait.jpg" alt="Dmitry Gofman" />
```
or replace the `builder-image` figure in the Builder's Path section.

---

## Sections

1. **Hero** — `ENGINEER. BUILDER. SEEKER.`
2. **Worldview** — practical mind / future-facing compass
3. **Engineering** — 4 capability cards + expandable professional background
4. **Builder's Path** — workshop / craft / hardware narrative
5. **Human Dimension** — people, teams, culture
6. **Vision** — future studio direction
7. **Contact** — email, LinkedIn, GitHub

## Design system

- **Background**: `#0A0A0A` (deep charcoal)
- **Text**: `#F4F4F0` (off-white)
- **Accents**: copper `#B87333`, clay `#A47551`, sand `#D6B89E`, olive `#5B6651`
- **Typography**: Fraunces (serif headings), Inter (body), JetBrains Mono (eyebrows/labels)
- **Decoration**: blueprint grid, CAD geometry, registration corner ticks
