# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Marketing landing page for PICAsell — a luxury recommerce platform. Hosted via GitHub Pages at `picasell.eu` (configured via CNAME file).

## Architecture

- **Single file site**: Everything lives in `index.html` — HTML, CSS (in `<style>` tag), and inline SVG icons. No build step, no JavaScript framework, no external dependencies beyond Google Fonts.
- **No build/test/lint commands**: Open `index.html` directly in a browser to preview.
- **Fonts**: Playfair Display (headings) and Inter (body) loaded from Google Fonts.

## Brand Identity

- **Color palette**: Gold (`--gold-400: #FFD333` primary) and cream (`--cream: #FDFBF7` background) — matches the frontend app at `../picasell-frontend/`.
- **Typography**: Playfair Display for all headings (`h1-h4`), Inter for body text.
- **Tone**: Luxury, technical credibility, sustainability-focused.

## Sections

Hero, stats bar, capabilities (6 cards), how-it-works (3 steps), platform (features + API code sample), sustainability (3 cards), architecture (12 service cards), CTA, footer.

## Sibling Projects

- `../picasell/` — Go microservices backend (12 services: user, auth, product, order, auction, rental, payment, AI, blockchain, upload, analytics + Traefik gateway)
- `../picasell-frontend/` — React 19 + Vite + Tailwind frontend application

## Key Details

- Contact email: `hello@picasell.eu`
- `dashboard.jpg` is the hero image, referenced as `/dashboard.jpg` (absolute from site root).
- Responsive breakpoints: 1024px and 768px. Mobile nav uses a toggle button with inline JS.
- CSS custom properties defined in `:root` for the gold/cream palette.
