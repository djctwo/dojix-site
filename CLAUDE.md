# Dojix Website (dojix-site)

## Project
- **What**: Marketing website for Dojix — a native macOS trade journal for forex traders
- **Repo**: `https://github.com/djctwo/dojix-site` (branch: main)
- **Hosting**: GitHub Pages, custom domain `dojix.app`
- **Stack**: Static HTML, inline CSS, no build tools, no framework
- **Fonts**: DM Sans (body/headings) + JetBrains Mono (stats/prices/mono) via Google Fonts

## Pages
| Path | Purpose |
|------|---------|
| `index.html` | Homepage — hero, features overview, pricing, comparison table |
| `features/index.html` | All 10 feature showcases with screenshots + 66 analytics deep-dive |
| `support/index.html` | FAQ accordion with 20+ questions across 6 categories |
| `privacy/index.html` | Privacy policy |
| `terms/index.html` | Terms of service |
| `404.html` | Custom 404 page |

## Design System
- **Palette**: `--bg: #0e0d0b`, `--surface: #141310`, `--card: #1c1b18`, `--accent: #e8b44c` (warm gold), `--text: #e8e4dc`, `--muted: #9a9488`
- **Typography**: DM Sans for all text, JetBrains Mono for numbers/stats/code/tags
- **Cards**: `--card` bg with `--border` (8% opacity gold), hover to `--border-strong` (14%)
- **Hero showcases**: gold top border, `--surface` bg, "No competitor has this" tag
- **Nav**: sticky, blurred background, hamburger at 600px breakpoint

## Current State
- **Pre-launch**: All download buttons show "Coming Soon" with disabled styling
- **Rollback tag**: `pre-critique-redesign` at commit `f0eaadd` (original site before warm gold redesign)
- **SEO**: robots.txt, sitemap.xml, JSON-LD (Organization, SoftwareApplication, FAQPage), OG tags on all pages
- **Mobile**: hamburger nav on homepage, features, support; privacy/terms have simple "Back to Home"

## Design Critique History
- **Pre-redesign score**: 20/40 (Nielsen's 10 Heuristics), 7 AI slop tells
- **Post-redesign score**: 26/40, AI slop PASS, cognitive load reduced from 6/8 Critical to 3/8 Moderate
- All 5 post-redesign critique issues fixed (P1: download buttons, P1: features grouping, P2: mobile nav, P2: 404 page, P3: comparison table)

## SEO Status
### Phase 1 (Done)
- robots.txt + sitemap.xml
- JSON-LD Organization + SoftwareApplication schema (homepage)
- JSON-LD FAQPage schema with 6 questions (support)
- Meta descriptions, canonical URLs, OG tags on all pages

### Phase 2-4 (Future)
- Blog content: Monte Carlo, Kill Zones, Risk of Ruin guides
- Comparison landing pages: `/alternatives/tradersync/`, `/tradervue/`, `/edgewonk/`
- Primary keywords: "forex trade journal", "trade journal for mac", "best trade journal app"
- Long-tail: "monte carlo simulation trading", "risk of ruin calculator forex", "TraderSync alternative"
- Backlink building: fintech blogs, forex communities, Product Hunt

## Conventions
- All pages use inline `<style>` blocks (no shared CSS file)
- Images in `/images/` directory
- Lightbox on pages with screenshots (features, homepage)
- Footer consistent across pages: Home, Features, Privacy, Terms, Support
- Legal entity: Aaxis Holdings Group LLC
