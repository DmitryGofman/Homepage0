# PRD — Dmitry Gofman Personal Brand Landing Page

## Original problem statement
Rebuild personal homepage at https://dmitrygofman.github.io/homepage as a professional personal-brand landing page (NOT a CV/resume). Core identity: **ENGINEER. BUILDER. SEEKER.** Multidisciplinary engineer working between physical systems, technology, craft, and human potential. Single static HTML/CSS/JS file deployable to GitHub Pages. No backend. mailto: contact only.

## Architecture
- Single self-contained `index.html` (HTML + embedded CSS + embedded JS).
- Deliverable path: `/app/site/index.html` + `/app/site/README.md` (deployment guide).
- Preview-environment mirror: `/app/frontend/public/index.html` (CRA serves it; React `App.js` renders `null`, `index.css` cleared so Tailwind base doesn't override).
- Google Fonts CDN: Fraunces / Inter / JetBrains Mono.

## User personas
- Recruiters / collaborators / founders / craftspeople landing on Dmitry's page wanting to quickly understand who he is and how to connect.

## Core requirements (static)
- Sticky minimal nav: Home, Worldview, Engineering, Builder's Path, Vision, Contact.
- Hero with headline `ENGINEER. BUILDER. SEEKER.`, subheadline, microcopy, dual CTAs.
- 4 engineering capability cards (R&D, Electromechanical, Manufacturing, Team & System Integration).
- Expandable "Professional background" panel.
- Builder's Path narrative + workshop image + tag cloud.
- Human Dimension grounded section with qualities grid.
- Vision section with numbered list + quote.
- Contact: mailto email, LinkedIn, GitHub.
- Smooth scroll, sticky nav, IntersectionObserver fade-ins, hover states.
- Mobile-first responsive (breakpoints at 880px and 760px).
- Design tokens: charcoal `#0A0A0A` bg, off-white `#F4F4F0` text, copper `#B87333`, clay, sand, olive accents. Blueprint grid background, CAD geometry, registration corner ticks.

## What's been implemented (Dec 2025)
- All 6 sections per brief (verbatim copy where specified).
- Static deliverable at `/app/site/index.html` ready to push to GitHub Pages.
- Preview rendering verified at https://dima-builder.preview.emergentagent.com.
- README with two deployment options (main branch root / gh-pages branch).
- **5 user-supplied photos integrated**: portrait card in hero (DVM 62), 3-image gallery in Builder's Path (forge / pottery wheel / studio render), wide handstand banner in Human Dimension, wide studio render in Vision.

## Backlog (P0/P1/P2)
- **P1**: Add Dmitry's portrait once user provides image (slot in hero or Builder's Path).
- **P1**: Optionally add an "open-source projects" or "writing" small section if user wants a destination beyond contact.
- **P2**: SEO meta + OG image (custom 1200×630 with copper/charcoal palette).
- **P2**: Subtle parallax on hero CAD geometry.
- **P2**: Custom 404 page matching the aesthetic for GitHub Pages.

## Next tasks
1. User uploads portrait → slot it into hero/Builder's Path.
2. User pushes `/app/site/index.html` to `dmitrygofman/homepage` (root or `gh-pages`).
