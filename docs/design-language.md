# Black Atom Design Language

## Creative North Star

"The Vault Terminal" — a technical, industrial aesthetic inspired by 1970s NASA documentation,
vintage product datasheets, and declassified government documents. The UI feels like an interface to
Black Atom's color preservation vault: precise, restrained, and quietly authoritative.

## Aesthetic References

- DHARMA Initiative (Lost) — mysterious corporate identity, vintage badges
- NASA 1970s identity — Futura mixed with technical type, worm/meatball duality
- Berkeley Mono specimen — box-drawing diagrams, hatched shadows, RFC-style schematics
- black-atom.industries website — bordered sections, monospace, datasheet layout

## Typography

- **Mono (primary):** All labels, navigation, status text, section headers, form fields. Uppercase
  with letterspacing for section headers. Berkeley Mono is the visual reference (shipping font TBD).
- **Display/sans (accent):** Headings, product names, theme names. Provides visual weight and
  distinguishes content from chrome.

## Color System

All colors derive from `@black-atom/core` OKLCH tokens. See `docs/tokens.md` for hex mappings.

- **Chrome is near-monochrome.** Dark grays on dark mode, warm off-whites on light mode.
- **Accent colors:** Muted green for synced/valid/active. Purple for selected/focused.
- **Content is the color.** In Livery, the theme palettes are the only vibrant elements. In other
  products, the content itself brings color — chrome never competes.
- **Light mode:** Paper-like warmth to backgrounds (not pure white).
- **Dark mode:** Deep teal-tinted charcoal (not pure black).

## Surfaces & Borders

- Bordered panels with visible 1px solid edges — the datasheet box aesthetic.
- No rounded corners (or minimal, 2px max). Squared-off is more technical.
- Subtle hatched/dotted patterns as decorative texture on non-interactive surfaces.
- Box-drawing-inspired dividers and separators where appropriate.
- Depth through tonal layering, not shadows.

## Recurring Motifs

- **The dot/circle:** Logo mark (a literal black dot = black atom), wordmark "o" replacement, bullet
  indicators.
- **Uppercase mono labels** with horizontal rules underneath (section header pattern).
- **Bordered boxes** as the primary container pattern.
- **Technical metadata** in margins — version numbers, timestamps, status indicators.

## Light / Dark Mode

Both are first-class. The design must work equally well in both appearances — the chrome adapts, the
structure stays identical. Light mode uses warm paper tones, dark mode uses teal-tinted charcoal.

## Component Conventions

- **Buttons:** Bordered rectangles, monospace text, no fill on secondary actions. `[ BACK ]` style.
- **Inputs:** 1px border, monospace placeholder text, validation indicators inline.
- **Toggles/checkboxes:** Minimal, square. No rounded switch tracks.
- **Cards/sections:** Bordered boxes with uppercase mono header + horizontal rule.
- **Status indicators:** Colored dot + monospace label. Green = synced/valid, purple = selected.

## Logo

A black dot (filled circle). Literal representation of "black atom." Already embedded in the
wordmark as the "o" in "atom." Works at every scale: favicon, app icon, watermark, badge.

## Related Issues

- [DES-25](https://linear.app/black-atom-industries/issue/DES-25) — Logo design
- [DES-26](https://linear.app/black-atom-industries/issue/DES-26) — Banner design
