Google Stitch Presentation (Slidev)

Overview
- Slide deck built with Slidev showcasing Google Stitch — an AI‑powered concept for generating mobile and web UIs.
- Primary source: `slides.md`. Uses the `seriph` theme, dark color schema, MDC syntax, and UnoCSS utilities.

Quick Start
- Prerequisites: Node.js 18+ (18 or 20 recommended)
- Preview locally (no global install):
  - In `OneDrive/桌面/google-stitch`, run: `npx slidev slides.md --open`
- Optional local CLI install:
  - `npm i -D @slidev/cli`
  - `npx slidev slides.md --open`

Build and Export
- Static site: `npx slidev build slides.md`
- Export PDF: `npx slidev export slides.md --output export.pdf`
- Export images: `npx slidev export slides.md --format png` (or `--format jpeg`)

Slide Outline
- Stitch (intro): AI‑Powered UI Generation for Mobile & Web
  - See `OneDrive/桌面/google-stitch/slides.md:31`
- What is Google Stitch: positioning and platform support
  - See `OneDrive/桌面/google-stitch/slides.md:55`
- How Stitch AI works: Intent Parsing + Code/Design Rendering (revealed via `v-click`)
  - See `OneDrive/桌面/google-stitch/slides.md:69`, `:75`, `:79`
- Mode: Standard vs Experimental, centered layout via per‑slide class
  - See `OneDrive/桌面/google-stitch/slides.md:83` (per‑slide `class`), `:87` (heading)
- Using: placeholder for usage visuals
  - See `OneDrive/桌面/google-stitch/slides.md:121`
- Thank You: centered content with Q&A note
  - See `OneDrive/桌面/google-stitch/slides.md:127` (per‑slide `class`), `:131`

Styling and Tech Notes
- Global frontmatter in `slides.md`:
  - `theme: seriph`, `background: https://cover.sli.dev`, `mdc: true`, `colorSchema: dark`
  - Fonts: Inter / Crimson Pro / JetBrains Mono
- UnoCSS usage via per‑slide `class:` frontmatter:
  - Intro slide gradient and centering — `OneDrive/桌面/google-stitch/slides.md:14`
  - Mode slide vertical centering — `OneDrive/桌面/google-stitch/slides.md:83`
  - Thank You slide grid centering — `OneDrive/桌面/google-stitch/slides.md:127`
- Interactivity and icons:
  - Click actions like `@click="$slidev.nav.next"`, editor shortcut `$slidev.nav.openInEditor()`
  - Icons such as `<carbon:arrow-right />`, `<carbon:edit />` (ensure icon support per Slidev docs)

Authoring Tips
- Slide separators must be exactly `---` (no trailing spaces), or parsing may fail.
- Avoid placing Markdown headings inside block‑level HTML (e.g., `<div>`). Use per‑slide `class:` for layout.
- When using `v-click`, wrap revealable content in its own block to prevent list/Markdown interplay issues.

Known Fixes Applied
- Normalized a slide separator and moved container layout to per‑slide `class:` so `# Mode` renders correctly.
- Centered the Thank You slide with `grid place-content-center text-center h-full`.

License
- For demo and learning purposes. Adjust attributions and licensing for external use as needed.

