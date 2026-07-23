# [Practice Name] — Pre-Opening Launch Strategy

Client proposal prepared by Generate Your Audience.
Warrnambool VIC · two-chair practice · opening late October 2026.

**Confidential.** Contains competitor analysis of named local
businesses. `robots.txt` and a `noindex` meta tag are in place to
keep this out of search results — leave both alone.

## Deploy

Single self-contained file. The GYA logo and favicon are embedded
as base64, so there are no image dependencies.

**GitHub Pages** — push to the repo, then Settings → Pages →
Deploy from branch → `main` / `root`.

**Vercel** — import the repo, framework preset "Other", no build
command, output directory `./`.

## Before sending

17 placeholders are highlighted in gold with a dotted underline.
Find and replace both, and the highlight disappears with them:

- `[Practice Name]`
- `[Dr Principal]`

Also confirm before sending: the opening date (§10 assumes
Monday 26 October — every countdown week shifts with it) and the
pricing in §12.

## Editing

Colours are CSS custom properties in `:root` at the top of the
file, derived from the GYA logo gradient:

| Token | Value | Used for |
|---|---|---|
| `--brand` | `#E1594B` | Display type, large numerals |
| `--brand-deep` | `#B8402F` | Small labels, section markers |
| `--rose` / `--orange` | `#F0607E` / `#E86840` | Gradient endpoints |
| `--grad` | rose → orange | Countdown, badges, accent bars |
| `--ink` | `#23202A` | Body and headings |
| `--bone` | `#F7F5F4` | Page background |
