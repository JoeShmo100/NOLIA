# Nolia Software — Website Spec

> Give this file to a Claude session working on any Nolia Software product. It contains everything needed to create a matching product reference file (like TOGETHER.md) that the nolia-site can use to build an accurate product card.

## What Is nolia-site?

A minimal landing page for **Nolia Software LLC** — the parent company. It lives at `nolia.software` and showcases all Nolia products. Each product gets a card that links out to its own site.

**Repo:** `github.com/JoeShmo100/NOLIA`
**Stack:** Static HTML/CSS served by Express on Railway
**Structure:**
```
nolia-site/
├── server.js              # Express static server (reads PORT from env)
├── package.json
├── public/
│   ├── index.html         # Single-page site
│   ├── style.css          # All styles
│   └── fonts/             # MuseoModerno variable font (accent)
├── TOGETHER.md            # Product reference for Together's card
└── NOLIA-SITE-SPEC.md     # This file
```

## The Site Design

- **Dark minimal** — near-black background (#0a0a0a), warm cream/magnolia accents
- **Floating magnolia petals** — subtle SVG petals drift down the background at ~3% opacity
- **Magnolia flower icon** in the header next to the "nolia" wordmark
- **Hero:** "Software that makes us more human" — the word "human" is highlighted in magnolia cream
- **Subtitle:** "We build tools that bring people closer together — in person, in play, in purpose."
- **Three product cards** in a grid (stacked on mobile, 3-col on desktop)
- **Footer:** "© 2026 Nolia Software LLC"

### Fonts
- **Accent font (headings, logo, product names):** MuseoModerno (variable weight, self-hosted)
- **Body font:** Inter (Google Fonts, weights 300-600)

### Color Tokens
```css
--bg:            #0a0a0a
--surface:       #141414
--border:        #222
--text:          #e8e4df
--text-muted:    #8a8580
--magnolia:      #F5E6D3      /* primary accent — cream/warm white */
--magnolia-soft: #D4A574      /* secondary accent — warm bronze */
--magnolia-glow: rgba(245, 230, 211, 0.08)  /* subtle background glow */
```

### Product Card Structure
Each product card has:
1. **Icon** — 48x48 rounded square with magnolia glow background, containing an SVG icon
2. **Product name** — MuseoModerno, 20px, weight 500
3. **Description** — Inter, 15px, weight 300, muted text, 1-2 sentences
4. **Status** — either "Visit site →" (magnolia color, links out) or "Coming soon" (muted, uppercase)

Live products are wrapped in an `<a>` tag. Coming-soon products are `<div>`s (no link).

## What I Need From Your Product

To add your product to the nolia-site, create a markdown file called `[PRODUCT_NAME].md` in the nolia-site root with the following sections:

```markdown
# [Product Name] — Product Reference

## What It Is
One paragraph explaining the product.

## One-Liner
A single sentence for the card description (keep under 25 words).

## Core Value Props
- Bullet points of who it helps and how

## How It Works
Numbered steps of the core user flow

## Key Features
- Bullet list of notable features

## Pricing Tiers (if applicable)
| Tier | Price | Who it's for |
|------|-------|-------------|

## Brand & Design Language

### Fonts
- Display/Logo: [font name]
- Body: [font name]

### Color Palette
| Token | Value | Usage |
|-------|-------|-------|

### Visual Vibe
A few sentences describing the look and feel.

## Tech Stack
What it's built with.

## Live URL
The production URL (or "not yet live").
```

### Why This Matters
The product reference file lets me (or another Claude session working on nolia-site) design an accurate card that reflects each product's actual personality — using the right icon style, description tone, and eventually linking to the right URL. Without it, the card is just a generic placeholder.

## Current Products

| Product | Status | Card Status | Reference File |
|---------|--------|-------------|---------------|
| **Together** | Live | Placeholder card, links out | `TOGETHER.md` ✓ |
| **Dropslide** | In development | Placeholder card, "Coming soon" | Needs `DROPSLIDE.md` |
| **Game Base** | In development | Placeholder card, "Coming soon" | Needs `GAMEBASE.md` |

## Company Info
- **Company:** Nolia Software LLC
- **Founded:** 2026, Maryland
- **Mission:** Software that makes us more human
- **Named after:** Magnolia (mag-**nolia**) — hence the flower motifs
