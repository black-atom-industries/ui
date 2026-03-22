# Google Stitch Reference

Design exploration for Black Atom UI using [Google Stitch](https://stitch.withgoogle.com/).

## Project

- **ID:** `11018168170664527349`
- **Model:** Gemini 3.1 Pro

## Screens

The project contains mockups for three Livery views in light and dark mode:

1. **Main View** — Three-panel theme browser (navigator, specimen, adapter status)
2. **Setup Wizard** — Step-by-step first-run configuration
3. **Settings** — Per-adapter configuration page

## Workflow Learnings

- **DESIGN.md** in Stitch is auto-generated from the prompt — serves as handoff artifact for coding
  agents
- **Edit API** creates new screen versions alongside originals (no delete via MCP)
- Set the **Design System** (Theme tab + DESIGN.md) before generating screens for best results
- Stitch generates HTML/CSS per screen, downloadable via `get_screen` API
- Intended pipeline: Stitch → Figma → Code, but we go Stitch → Code directly

## Prompts Used

### Initial generation prompt

> Design a desktop application called "Black Atom Livery" — a theme management tool for developer
> environments. Show three screens: the main view, a setup wizard, and a settings page. Both dark
> mode and light mode variants.
>
> Visual identity: Technical, industrial aesthetic inspired by 1970s NASA documentation, vintage
> product datasheets, and declassified government documents. Monospace typography as the backbone
> with a clean sans-serif display font for theme names only. Bordered panels with 1px solid edges,
> sharp corners (no rounded corners). Uppercase monospace section headers with horizontal rules
> underneath. Box-drawing-inspired separators and dividers. Minimal color in the UI chrome — the
> theme color palettes are the only vibrant elements. Dark mode uses deep charcoal (not pure black).
> Light mode uses warm off-white paper-like backgrounds (not pure white).
>
> Main view: Three-panel layout. Left: theme list grouped by collections (DEFAULT, JPN, TERRA) with
> uppercase headers, selected theme has left border accent. Center: large theme name "Fall Night" in
> display font, "dark" badge, description text, metadata row (APPEARANCE | COLLECTION | VARIANTS |
> PRIMARIES) in label-over-value format, and a row of 12 color swatches with tiny labels. Right:
> "ADAPTERS" panel showing app sync status — Ghostty, Neovim, Tmux, Delta each with a letter icon
> in a bordered square, "Synced" status, and dimmed reload method label. Bottom bar with green sync
> indicator dot and timestamp.
>
> Setup wizard: Step-by-step flow, "STEP 02 / 04 — CONFIGURATION" shown. List of detected apps with
> editable path inputs and validation checkmarks. Squared-off bordered navigation buttons [ BACK ]
> and [ NEXT ]. Fully datasheet aesthetic.
>
> Settings page: Vertical scroll, one bordered section per adapter. Each has: enabled toggle, config
> path input with validation, dimmed reload method label. Collapsible ADVANCED section. Fully
> utilitarian technical document style.

### Revision prompt (v2 — muted palette)

> Revise all screens. The current design is too colorful and garish. Pull back dramatically toward
> the aesthetic of a vintage printed technical document — think plain text on warm cream paper in
> light mode, muted monochrome terminal on deep charcoal in dark mode. The only accent color should
> be a single muted green for "synced/valid" status indicators. Remove the red entirely. No charts
> or data visualizations. Buttons should be simple bordered rectangles with monospace text, not
> filled colored blocks. The feel should be quiet, austere, and restrained — like an old RFC document
> or a product datasheet from a 1970s electronics catalog. Let the theme color palette swatches be
> the ONLY vibrant color on the entire screen. Everything else is black, white, and warm grays.
