# [Practice Name] — Pre-Opening Launch Strategy

Client proposal prepared by Generate Your Audience.
Warrnambool VIC · two-chair practice · opening late October 2026.

**Confidential.** Contains competitor analysis of named local
businesses. `robots.txt` and a `noindex` meta tag are in place to
keep this out of search results — leave both alone. Keep the repo
private; §13 has pricing in it.

## Deploy

**GitHub Pages** — push, then Settings → Pages → Deploy from
branch → `main` / `root`.

**Vercel** — import the repo, framework preset "Other", no build
command, output directory `./`.

## Before sending

17 placeholders are highlighted in gold with a dotted underline.
Find and replace both and the highlight goes with them:

- `[Practice Name]`
- `[Dr Principal]`

Also confirm: the opening date (§11 assumes Monday 26 October —
every countdown week shifts with it) and the pricing in §13.

## Portfolio carousel (§10.1)

Five live GYA builds. Screenshots are in `assets/shots/`, cropped
to 1600 × 696 (23:10, a wide desktop viewport) and saved as
progressive JPEG. To swap one out, keep the filename and the
dimensions:

| File | Site |
|---|---|
| `01-horizon.jpg` | Horizon Dental — Sydney CBD |
| `02-artarmon.jpg` | Artarmon Dentists — Artarmon NSW |
| `03-grey-street.jpg` | Grey Street Dentist — St Kilda VIC |
| `04-synergy.jpg` | Synergy Dental Group — Parkdale VIC |
| `05-tooth-n-care.jpg` | Tooth n Care — East Maitland NSW |

No URLs appear anywhere in the carousel — the browser tab shows
the practice name and location only, so staging links stay
private.

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
(`@keyframes rule-sweep`). Both disable automatically under
`prefers-reduced-motion`.
