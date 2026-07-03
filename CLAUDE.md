# OpenComp Website

Static company website for OpenComp Oy, served at **opencomp.fi** via GitHub Pages (see `CNAME`).

## Hard constraints — never violate these

1. **The site must remain a purely static website.**
   - No build tools, bundlers, or preprocessors (no npm, Vite, Webpack, Sass, Tailwind, etc.).
   - No dependencies: no `package.json`, no frameworks (React, Vue, jQuery, ...), no CDN-loaded libraries.
   - All code is plain **HTML**, **CSS**, and **native (vanilla) JavaScript** only.
   - Every page must work by opening the `.html` file directly — no server-side logic, no build step.

2. **Follow the design system in `DESIGN.md` at all times.**
   - `DESIGN.md` defines the "Solo Authority" design system: colors, typography (Manrope), spacing, shapes, and component rules.
   - When creating new pages or components, use the existing CSS custom properties in `css/style.css` (e.g. `--accent`, `--surface-container`, `--stack-lg`) instead of hard-coding values.
   - Dark "Deep Slate" theme is the default and only theme. Accent color Forest Teal (`--accent: #2dd4bf`) is used sparingly: CTAs, active states, highlights.
   - Depth via tonal layers and 1px `--outline-variant` borders — no drop shadows.

## Structure

- `index.html` — landing page (Finnish, primary)
- `articles.html` — article listing (Finnish, primary). Currently hidden from navigation until real article content exists — restore the nav link on all pages when articles are published.
- `cv.html` — professional timeline / CV (Finnish, primary)
- `en/` — English versions of all pages (`en/index.html`, `en/articles.html`, `en/cv.html`)
- `css/style.css` — single stylesheet for the whole site; design tokens as CSS variables in `:root`
- `images/` — logos and images
- `DESIGN.md` — design system specification (source of truth for styling)
- `CNAME` — GitHub Pages custom domain, do not modify or delete

## Languages

- **Finnish is the primary language**: Finnish pages live at the site root, English mirrors under `en/`.
- Every page has a FI/EN language switcher in the header (`.lang-switch`) linking to its counterpart page — a new page must always be created in both languages.
- Content changes must be applied to **both** language versions to keep them in sync.
- Set `<html lang="fi">` / `<html lang="en">` and the `hreflang` alternate links in `<head>` accordingly.
- English pages reference shared assets with relative paths (`../css/style.css`, `../images/...`).

## Conventions

- Shared header/nav markup is duplicated in every page (no templating) — when changing navigation, update **all** HTML pages consistently.
- Keep styles in `css/style.css`; avoid inline styles in HTML.
- Mobile breakpoint is `768px`; new components must be responsive.
- Contact email is `contact@opencomp.fi`.
