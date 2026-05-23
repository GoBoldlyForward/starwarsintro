# Changelog

## 1.1.0 — 2026-05-23

Demo page refresh. Plugin CSS (`starwarsintro.css`) is unchanged.

### Changed
- Demo adopts the shared Go Boldly Forward plugin design system:
  - Light + dark mode via `prefers-color-scheme`
  - Inter typography (rsms.me); system stack fallback
  - `.gbf-*` markup convention (`.gbf-header`, `.gbf-section`, `.gbf-canvas`, `.gbf-code`, `.gbf-footer`)
  - Yellow accent (`#ca8a04` light / `#facc15` dark) matching the crawl text
- Crawl is scoped to a bounded 75vh stage on the demo so the chrome around it can adapt to light/dark; the crawl itself stays on its dark space backdrop.

### Added
- `demo.css` — synced copy of the canonical theme at `~/code/_plugins/_shared/demo.css`.

## 1.0.0 — 2025

Modernization release. First publication under the Go Boldly Forward name.

### Changed
- Rebrand: Polar Notion → Go Boldly Forward (CSS header, package metadata).
- Strip obsolete vendor prefixes (`-webkit/-moz/-ms/-o`); fix broken gradient syntax.

### Removed
- Demo page no longer depends on jQuery, Bootstrap, or JotForm. Native CSS smooth-scroll.
- Legacy artifacts: `.DS_Store`, `starwarsintro.css.zip`.

### Added
- `LICENSE` (MIT), `README.md`, `package.json`, `.gitignore`.
- Scoped npm name `@goboldlyforward/starwarsintro` with `publishConfig.access: public`.
