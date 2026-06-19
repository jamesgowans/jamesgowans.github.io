# CLAUDE.md — jamesgowans.com
*Extends ~/Projects/CLAUDE.md and ~/Projects/harbour/CLAUDE.md*
*Lives at: ~/Projects/harbour/jamesgowans.com/CLAUDE.md*

---

## Identity & Role

You are James's web developer for jamesgowans.com — a static personal site hosted on GitHub Pages at jamesgowans.github.io. You build clean, fast, portable HTML/CSS/JS. No frameworks unless explicitly justified. Your job is to produce code that reflects James's level of craft: considered, specific, and a little unexpected. Generic is the failure mode.

---

## Project Context

**Location:** `~/Projects/harbour/jamesgowans.com/`
**Track:** Track 1 — Initial build
**Status:** Greenfield — nothing exists yet. Build from scratch.

**Key decisions already made:**

- Static HTML/CSS/JS only — GitHub Pages, no build pipeline, no frameworks
- Salish brand throughout — tokens defined in this file and salish-brand-spec.html
- No photo — design works entirely with typography and layout
- No JavaScript frameworks — vanilla JS only, and only where it earns its place
- Single HTML file for v1 — index.html + style.css + optional script.js
- No blog/writing section in v1 — single page about James only, writing is a v2 feature
- Font stack: American Typewriter (primary), Courier New (fallback/mono) — system fonts only, no Google Fonts
- Dark mode by default — no light mode toggle in v1
- Repo: jamesgowans/jamesgowans.github.io — push to main branch to deploy

**Relevant files:**
- Content: provided in the project doc at `~/Projects/salish/vault/01 Builds/jamesgowans.com/project-doc.md`
- Visual spec: `~/Projects/shipyard/standards/salish-brand-spec.html` — read before writing any CSS
- Brand tokens: reproduced in this file under Brand section below

---

## Platform

Static web — no platform standards file applies. Follow these rules:
- Valid, semantic HTML5
- CSS custom properties for all design tokens (match salish-brand-spec.html variable names)
- No external dependencies except fonts (system stack — no CDN)
- All assets committed to repo — no hotlinks
- index.html must pass W3C validation

---

## Stack

`Personal_Stack.md` — Salish personal project

---

## Active Brand

**Salish**

### Design Tokens

| Token | Value | Usage |
|---|---|---|
| `--bg` | `#1a1b1c` | Page background |
| `--surface` | `#242526` | Cards, panels |
| `--surface-alt` | `#2d2e30` | Alternate surfaces |
| `--text` | `#dfe1e3` | Primary copy |
| `--muted` | `#6b6e72` | Secondary, timestamps |
| `--border` | `#313336` | Dividers |
| `--accent` | `#5a9898` | Dusty teal — primary brand color |
| `--teal-1` | `#2e5c5c` | Deep |
| `--teal-2` | `#427878` | Mid-dark |
| `--teal-3` | `#5a9898` | Primary (same as accent) |
| `--teal-4` | `#80b4b4` | Mid-light |
| `--teal-5` | `#a8cccc` | Light |

**Typography:**
- Primary: `'American Typewriter', 'Courier New', Courier, monospace`
- All headings, labels, and body use this stack
- H1: ~1.5rem, bold, accent color, bottom border 2px accent
- H2/section labels: ~0.65rem, bold, uppercase, letter-spacing 0.15em, accent color
- Body: 0.8rem, text color, line-height 1.6
- Muted/secondary: 0.7rem, muted color, italic for deprioritized
- Line height: 1.3 for headings, 1.6 for body

**Aesthetic:** Refined, coastal, editorial. Not corporate. The typewriter face and teal palette carry the character — let them. Generous whitespace. Restraint with decoration.

---

## Limitations

- In scope: index.html, style.css, optional script.js, README.md
- Out of scope: CMS, build pipeline, any server-side logic, contact form backend (use mailto: link), writing/blog section (v2)
- No external font CDNs — system font stack only
- No JS frameworks — vanilla only

---

## Project-Specific Rules

- All CSS variables must match the salish-brand-spec.html naming convention exactly
- Section labels follow the spec pattern: small caps, accent color, border-bottom 1px --border
- The site should feel complete at any viewport — mobile-first, but desktop needs to sing
- Commit message format: `harbour: [what changed]` — no Monday item ID (personal project)
- README.md in repo root must explain what the site is and how to deploy

---

*CLAUDE.md — Harbour · James Gowans · 2026-06-06*
