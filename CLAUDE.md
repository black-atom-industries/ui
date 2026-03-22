# @black-atom/ui

Shared UI component library for Black Atom products. Published on JSR as `@black-atom/ui`.

## Architecture

- **BaseUI** (headless) for accessible component primitives
- **CSS Modules** for component styling — no Tailwind
- **CSS custom properties** mapped from `@black-atom/core` design tokens (OKLCH)
- **Deno** runtime, published via JSR

## Consumers

- **Livery** — Tauri desktop app for theme management
- **black-atom.industries** — Website
- **nbr.haus** — Personal site

## Design Language

See `docs/design-language.md` for the full spec. Key principles:

- Technical/industrial aesthetic — vintage datasheets, 1970s NASA documentation
- Monospace typography backbone + display sans for headings
- No rounded corners. 1px borders. Uppercase mono section headers.
- Chrome is monochrome — themes bring the color
- Light and dark mode both first-class

## Project Tracking

Issues tracked in [Linear](https://linear.app/black-atom-industries) under the **ui** project.

## Sources of Truth

- **@black-atom/core**: https://jsr.io/@black-atom/core
- **BaseUI**: https://base-ui.com/
- **Deno**: https://docs.deno.com/
