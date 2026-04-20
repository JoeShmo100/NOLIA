# Together — Product Reference

Use this file to design an accurate product card on the Nolia site.

## What It Is
An event photo/video challenge app for weddings, parties, and live events. Guests scan a QR code, enter their name, and get a curated list of photo/video challenges. Media uploads in real-time to a live slideshow at the venue. The host walks away with a crowd-sourced photo/video collection organized by challenge.

## One-Liner
Photo scavenger hunts for weddings, parties, and events.

## Core Value Props
- **For guests:** A fun, guided way to participate and capture memories — no app download
- **For hosts:** A beautiful, automatic photo collection + a live slideshow moment during the event
- **For pros:** White-label, multi-event management, partner commissions

## How It Works (Guest Flow)
1. Scan QR code at the event
2. Enter name + last 4 digits of phone
3. See challenge list (e.g. "Capture the first dance", "Find someone in a hat")
4. Take photos/videos directly or upload from library
5. Submissions appear live on the slideshow

## Key Features
- AI-generated challenges (powered by Claude Haiku)
- Live slideshow with continuous scroll engine
- Wedding-specific mode with time slots (ceremony, reception, etc.)
- Gallery for browsing + downloading all submissions
- Multi-language (English + Spanish)
- Shared dashboard for co-hosts
- QR card generator (print-ready)
- Accent color customization (paid tiers)

## Pricing Tiers
| Tier | Price | Who it's for |
|------|-------|-------------|
| Free | $0 | Try it out — 20 guests, 5 challenges |
| Party | $39 one-time | Birthday, reunion, corporate |
| Wedding Day | $149 one-time | Full wedding with time slots |
| Host | $69/month | Recurring party hosts |
| Pro | $299/month | Coordinators, photographers |
| Venue | $699/month | Venues, full white-label |

## Brand & Design Language

### Fonts
- **Display/Logo:** Shrikhand (bold, warm, playful)
- **Body:** Inter (clean, modern)

### Color Palette (Dark Mode — Default)
| Token | Value | Usage |
|-------|-------|-------|
| `--bg` | `#0d0d0d` | Page background |
| `--surface` | `#161616` | Card backgrounds |
| `--surface-2` | `#1f1f1f` | Elevated surfaces |
| `--text` | `#f0efec` | Primary text |
| `--text-muted` | `#77776e` | Secondary text |
| `--accent` | `#ffc600` | Primary accent (gold/amber) |
| `--accent-2` | `#ff9400` | Secondary accent (orange) |

### Color Palette (Light Mode)
| Token | Value |
|-------|-------|
| `--bg` | `#fafaf9` |
| `--surface` | `#ffffff` |
| `--surface-2` | `#f4f3f0` |
| `--text` | `#1a1918` |
| `--text-muted` | `#6b6966` |
| `--accent` | `#ffc600` |
| `--accent-2` | `#ff9400` |

### Visual Vibe
- Dark by default, warm amber/gold accents
- Mobile-first (guests are on phones)
- Playful but not childish — think "fun wedding energy"
- Rounded corners, soft surfaces, generous spacing
- The Shrikhand logo font gives it personality vs. the clean Inter body

## Tech Stack
- React + Vite (frontend)
- Node.js + Express (backend)
- PostgreSQL via Prisma
- Socket.io (real-time)
- Cloudinary (media)
- Railway (hosting)

## Live URL
https://together.nolia.software (pending domain setup)
