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

- `index.html` — landing page
- `articles.html` — article listing
- `cv.html` — professional timeline / CV
- `css/style.css` — single stylesheet for the whole site; design tokens as CSS variables in `:root`
- `images/` — logos and images
- `DESIGN.md` — design system specification (source of truth for styling)
- `CNAME` — GitHub Pages custom domain, do not modify or delete

## Conventions

- Shared header/nav markup is duplicated in every page (no templating) — when changing navigation, update **all** HTML pages consistently.
- Page content language is English.
- Keep styles in `css/style.css`; avoid inline styles in HTML.
- Mobile breakpoint is `768px`; new components must be responsive.
- Contact email is `contact@opencomp.fi`.
