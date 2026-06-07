# jamesgowans.com

Personal site for James Gowans — Sr Manager, Technology Operations, Cactus Club Cafe.

## What It Does

Single-page personal site. Four sections: Hero, About, Experience, Contact. No framework, no CMS, no build step — just HTML, CSS, and GitHub Pages.

## How It Works

Static files served directly by GitHub Pages from the `main` branch of `jamesgowans/jamesgowans.github.io`. No preprocessing, no dependencies.

## Files

| File | Purpose |
|---|---|
| `index.html` | Single-page site — all content |
| `style.css` | All styles — Salish design tokens, layout, typography |
| `README.md` | This file |
| `CLAUDE.md` | Project configuration for Claude Code sessions |

## Inputs / Outputs

No inputs. Output: `https://jamesgowans.github.io` — publicly accessible via GitHub Pages.

## How to Deploy

Push to `main`. GitHub Pages auto-deploys within ~60 seconds.

```bash
git add .
git commit -m "harbour: [what changed]"
git push origin main
```

GitHub Pages is configured to serve from the root of `main` — no settings change required.

## Configuration

All design tokens are CSS custom properties in `style.css` `:root`. To update brand colors or typography, edit the `:root` block. Token names match `salish-brand-spec.html` exactly.

Content lives in `index.html` — update text directly, no templates or data files.

## Known Limitations

- No writing/blog section — v2 feature
- No dark/light mode toggle — dark mode only
- No photo — typographic design only
- Contact via mailto: link only — no form backend

## Version

v1 · 2026-06-06
