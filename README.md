# Thabang — Portfolio

Personal portfolio website built with vanilla HTML/CSS/JS following the uicode canonical
portfolio spec (dark theme, single amber accent, scroll-reveal, skill bars, typing effect).
No framework, no build step, no external font CDN.

## Sections
- **Hero** — Name + animated typing roles (Web Developer / Freelance Designer /
  Small-Business Owner / Automation Builder), GitHub / WhatsApp / email links, CTAs.
- **About** — Bio (how-I-think framing), info list, SiteCraft SA + Come & Buy Enterprise.
- **Stats** — honest offer facts (R1,500 setup, R450/mo, owner-editable, R0 hosting).
- **Services** — What I Build: done-for-you sites, custom builds, local SEO, automation.
- **Skills** — 6 competencies with honest, scroll-filled progress bars (no 100%).
- **Work** — Filterable project grid (All / Web / Business / Automation) with real projects.
- **Process** — Discover → Build → Launch → Support.
- **FAQ** — plain-language answers to common client questions.
- **Contact** — mailto form + details (lehauthabang@gmail.com, +27 74 508 6001, GitHub).
- **Footer** — socials, auto year, back-to-top.

## Files
- `index.html` — markup (expanded single-page site)
- `style.css` — styles (single accent `--accent: #f59e0b`, system font stack)
- `script.js` — sticky nav, mobile menu, active-link observer, typing, reveal + skill fill,
  project filtering, back-to-top, auto year
- `favicon.svg` — amber "T" monogram tab icon
- `AGENTS.md` — agent/AI coding rules for this project

## Robustness
- Hidden state gated on `.js` class in `<head>` so content is always visible if JS fails.
- In-viewport elements revealed synchronously; `IntersectionObserver` only for below-fold.
- `prefers-reduced-motion` safe.

## Fill-ins still needed (search `TODO(Thabang)` in index.html)
- Real portrait at `img/me.jpg` (or keep the "T" monogram).
- CV PDF URL on the Download CV button.
- Real live/repo URLs for SiteCraft client demo + Come & Buy storefront.
- 3+ more real projects.

## Local dev
```bash
python3 -m http.server 8123
# open http://localhost:8123/
```

## Deploy
GitHub Pages → thabs1234.github.io/portfolio. (Note: setting a custom domain 301-redirects
the github.io URL; confirm DNS before pointing.)
