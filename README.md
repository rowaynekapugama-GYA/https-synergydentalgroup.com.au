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

## ⚠️ Replace the portfolio screenshots

§10.1 has a carousel of five GYA builds. It currently shows
labelled placeholders that say REPLACE THIS FILE. Overwrite each
with a real screenshot, keeping the exact filename:

| File | Site |
|---|---|
| `assets/shots/01-horizon.png` | Horizon Dental |
| `assets/shots/02-artarmon.png` | Artarmon Dentists |
| `assets/shots/03-grey-street.png` | Grey Street Dentist |
| `assets/shots/04-synergy.png` | Synergy Dental Group |
| `assets/shots/05-tooth-n-care.png` | Tooth n Care |

**Target 1600 × 1000 px**, desktop homepage, full-page or
above-the-fold. The frame crops to 16:10 from the top, so the
hero should sit in the top portion. No URLs appear anywhere in
the carousel — the browser tab shows the practice name only, so
staging links stay private.

Quickest capture: Chrome → F12 → Ctrl/Cmd+Shift+M → set 1600×1000
→ ⋮ menu → Capture screenshot.

## Before sending

17 placeholders are highlighted in gold with a dotted underline.
Find and replace both and the highlight goes with them:

- `[Practice Name]`
- `[Dr Principal]`

Also confirm: the opening date (§11 assumes Monday 26 October —
every countdown week shifts with it) and the pricing in §13.

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
(`@keyframes neon-spin`) and the hero rule uses a travelling
sweep (`@keyframes rule-sweep`). Both are disabled automatically
under `prefers-reduced-motion`.
