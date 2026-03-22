# @black-atom/ui

Shared UI component library for [Black Atom Industries](https://github.com/black-atom-industries) products.

## Status

**Pre-development** — This repo currently contains design documentation and project scaffolding.
Components will be extracted from [Livery](https://github.com/black-atom-industries/livery) once
UI patterns stabilize.

## Tech Stack

- [BaseUI](https://base-ui.com/) — Headless component primitives
- CSS Modules — Component styling
- [Deno](https://deno.com/) — Runtime
- [JSR](https://jsr.io/@black-atom/ui) — Package registry

## Design Tokens

All colors and design tokens derive from
[@black-atom/core](https://jsr.io/@black-atom/core), which defines themes in OKLCH color space.

## Consumers

- **Livery** — Theme management desktop app (Tauri)
- **black-atom.industries** — Website
- **nbr.haus** — Personal site
