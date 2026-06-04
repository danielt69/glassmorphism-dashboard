# Glassmorphism Dashboard

A polished, responsive glassmorphism analytics dashboard UI — pure HTML/CSS with a touch of vanilla JS, no backend.

**Live demo → https://danielt69.github.io/glassmorphism-dashboard/**

![Pure HTML/CSS/JS](https://img.shields.io/badge/stack-HTML%20%2B%20CSS%20%2B%20vanilla%20JS-6d8bff) ![No build step](https://img.shields.io/badge/build-none-34d399) ![Single file](https://img.shields.io/badge/file-single%20index.html-b06dff)

A premium-SaaS-style dashboard mock that shows off layout and modern aesthetic craft: a CSS-grid app shell, frosted-glass panels over animated gradient blobs, KPI cards with trend deltas, hand-drawn SVG charts (no chart library), and a transactions table.

## Highlights

- **Glassmorphism done right** — `backdrop-filter: blur()` frosted panels, subtle borders, soft shadows, layered over a rich animated gradient-blob background.
- **Persistent dark / light theme** — toggled via CSS variables and tiny vanilla JS, saved to `localStorage` (defaults to your system preference on first visit).
- **Fully responsive** — clean three-column shell on desktop; the sidebar collapses into a slide-in drawer with a hamburger and scrim at mobile widths (tested at 390px).
- **No dependencies, no build step** — one self-contained `index.html` with inline `<style>` + `<script>`. Inline SVG icons and inline-SVG charts only.
- **Accessible & motion-safe** — semantic landmarks, ARIA labels, keyboard-dismissable drawer, and full `prefers-reduced-motion` support.

## How it works

- Everything lives in a single `index.html` — markup, styles, and script are inline.
- The **theme toggle persists** across reloads via `localStorage` and falls back to `prefers-color-scheme`.
- The layout is **fully responsive**: a CSS-grid shell on desktop and a JS-driven drawer nav on small screens.
- The bar chart is generated with a few lines of vanilla JS that emit inline `<svg>` `<rect>` elements — **no chart library**.
- It's a **static mock**: no backend, no network calls, no real data.

## Run locally

Just open the file — no server or build required:

```bash
open index.html
```

## Tech

Hand-written HTML, modern CSS (grid, custom properties, `backdrop-filter`), and a small slice of vanilla JavaScript. Zero frameworks, zero dependencies.
