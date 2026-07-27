# Lava Street Dental — Pre-Opening Launch Strategy

Client proposal prepared by Generate Your Audience.
Lava Street, Warrnambool VIC · two-chair practice · opening
late October 2026 · principal Dr Meg.

**Confidential.** Contains competitor analysis of named local
businesses. `robots.txt` and a `noindex` meta tag keep this out of
search results — leave both alone. Keep the repo private; §12 has
pricing in it.

## Deploy

**GitHub Pages** — push, then Settings → Pages → Deploy from
branch → `main` / `root`.

**Vercel** — import the repo, framework preset "Other", no build
command, output directory `./`.

## Before sending

Practice name (Lava Street Dental) and principal (Dr Meg) are set
throughout. Two things left to confirm:

- **Opening date** — §10 (the six-week countdown) assumes Monday
  26 October. Every countdown week shifts with it; tell me the
  real date and I'll re-cut the schedule.
- **Pricing** — the numbers in §12 are carried across from an
  earlier proposal. Sanity-check before it goes out.

## Portfolio carousel (§9.1)

Five live GYA builds. Screenshots are in `assets/shots/`, cropped
to 1600 × 696 and saved as progressive JPEG. To swap one, keep
the filename and dimensions:

| File | Site |
|---|---|
| `01-horizon.jpg` | Horizon Dental — Sydney CBD |
| `02-artarmon.jpg` | Artarmon Dentists — Artarmon NSW |
| `03-grey-street.jpg` | Grey Street Dentist — St Kilda VIC |
| `04-synergy.jpg` | Synergy Dental Group — Parkdale VIC |
| `05-tooth-n-care.jpg` | Tooth n Care — East Maitland NSW |

No URLs appear in the carousel — the browser tab shows the
practice name and location only, so staging links stay private.

## Section map

1 Executive summary · 2 About GYA · 3 Starting position ·
4 The Warrnambool market · 5 Competitor landscape ·
6 Positioning · 7 Channel analysis · 8 The plan ·
9 Website build · 10 Six-week countdown · 11 First 90 days ·
12 Investment · 13 Why GYA · 14 Next steps

## Editing

Colours are CSS custom properties in `:root`, derived from the
GYA logo gradient.

| Token | Value | Used for |
|---|---|---|
| `--brand` | `#E1594B` | Display type, large numerals |
| `--brand-deep` | `#B8402F` | Small labels, section markers |
| `--rose` / `--orange` | `#F0607E` / `#E86840` | Gradient endpoints |
| `--grad` | rose → orange | Countdown, badges, accent bars |
| `--ink` | `#23202A` | Body and headings |
| `--bone` | `#F7F5F4` | Page background |

The hero countdown uses a rotating conic-gradient border
(`@keyframes neon-spin`); the hero rule uses a travelling sweep
(`@keyframes rule-sweep`). Both disable under
`prefers-reduced-motion`.
