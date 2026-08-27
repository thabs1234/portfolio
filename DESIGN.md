---
version: alpha
name: Thabang Portfolio
description: Editorial cream/orange design system for Thabang's portfolio (SiteCraft SA, Come & Buy, DealFinder SA) — adopted from a Dmitry Glukhovsky editorial style.
colors:
  primary: "#fa5d29"
  secondary: "#e0471a"
  tertiary: "#fbe1d4"
  neutral: "#faf4eb"
  surface: "#fffdfa"
  surface-2: "#f1e8da"
  ink: "#402100"
  muted: "#7a6a55"
  line: "#e7dccb"
  on-accent: "#ffffff"
typography:
  h1:
    fontFamily: Noto Serif, Georgia, Times New Roman, serif
    fontSize: 3.2rem
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: "-0.01em"
  h2:
    fontFamily: Noto Serif, Georgia, Times New Roman, serif
    fontSize: 2rem
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: "-0.01em"
  body-md:
    fontFamily: Inter Tight, Poppins, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, sans-serif
    fontSize: 1rem
    fontWeight: 400
    lineHeight: 1.6
rounded:
  sm: 6px
  md: 8px
  lg: 12px
  xl: 16px
spacing:
  sm: 14px
  md: 22px
  lg: 48px
  section: 90px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-accent}"
    rounded: "{rounded.sm}"
    padding: 12px
  button-primary-hover:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-accent}"
  card-surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.lg}"
    padding: 18px
  card-surface-2:
    backgroundColor: "{colors.surface-2}"
    textColor: "{colors.muted}"
    rounded: "{rounded.lg}"
    padding: 18px
  nav-link-active:
    textColor: "{colors.primary}"
  divider:
    backgroundColor: "{colors.line}"
  app-background:
    backgroundColor: "{colors.neutral}"
---

## Overview

An editorial design system for Thabang Lehau's portfolio and client sites
(SiteCraft SA, Come & Buy Enterprise, DealFinder SA). Warm paper-cream canvas
(`#faf4eb`), dark-brown ink (`#402100`), and a single SiteCraft **orange**
accent (`#fa5d29`). Display type is Noto Serif; body is Inter Tight. The look
is free-only — Google Fonts via `<link>`, no paid license — and is reused across
client builds so the brand stays consistent.

## Colors

- **Primary (#fa5d29):** SiteCraft orange. The only accent — CTAs, links, active
  nav, scroll-progress bar, card hovers, stat numbers.
- **Secondary (#e0471a):** deeper orange for hover/pressed states.
- **Tertiary (#fbe1d4):** soft orange tint for chips/highlights behind text.
- **Neutral (#faf4eb):** page background (warm paper). **Surface (#fffdfa) /
  Surface-2 (#f1e8da):** cards and alternating panels. **Ink (#402100):** all
  text. **Muted (#7a6a55):** secondary text. **Line (#e7dccb):** hairline
  borders.

## Typography

Noto Serif for headings (editorial, humanist), Inter Tight for UI/body — with a
full system fallback so it renders even if the web font is blocked. Headings are
large and tight (`letter-spacing: -0.01em`); body is comfortable at 1rem/1.6.

## Components

`button-primary` is the high-emphasis action (solid orange, white text). Cards are
cream panels that lift and pick up the orange border on hover. `card-surface` and
`nav-link-active` are defined so agents reuse the exact tokens instead of
re-typing hex.

## Do's and Don'ts

- Do keep exactly one accent (orange). Don't introduce a second hue or indigo/violet.
- Do use the warm cream canvas + brown ink + serif display combo. Don't revert to
  a dark theme or cyan accent on this build.
- Do keep Noto Serif for headings only; Inter Tight for body. Don't swap the roles.
- Don't add vanity metrics; the stats band shows real offer facts (R1,500 / R450 / etc.).
