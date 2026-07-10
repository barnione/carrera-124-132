## Quick draft with claude, part-tested

# Carrera Control Unit Guide

A single-page, printable reference for programming the Carrera DIGITAL 124/132 Control Unit (item no. 30352), the black box that powers the track and handles all car programming.

The official manual ships as a dense multilingual PDF that's painful to use trackside. This page condenses the English instructions into one scrollable sheet: coding cars to controllers, setting top speed / braking / fuel tank, Pace Car and ghost car programming, factory reset, and a short troubleshooting table.

## Design

The page is styled after the printed service sheets that come in the Carrera box rather than a generic docs theme:

- Paper background, black ink, one spot color (Carrera red `#e2231a`)
- Barlow Condensed for headings, Archivo for body, IBM Plex Mono for item numbers, key names and figure labels
- Table of contents with dotted leaders, `Tab. x.x` / `Fig. x.x` numbering
- LED state figures: small diagrams showing what the Control Unit's five LEDs actually display at each step (solid / flashing / half-steps), since that's how the unit communicates
- A checkered finish-line strip in the masthead, borrowed from the track itself

Flashing LED animations respect `prefers-reduced-motion`, and the page prints reasonably if you want a physical copy next to the track.

## Usage

No build step, no dependencies to install. Everything is one file.

```
open carrera-digital-control-unit-guide.html
```

Or host it anywhere static (GitHub Pages, Cloudflare Pages, a folder on your NAS).

The only external requests are three Google Fonts. If you need it fully offline, replace the `<link>` tags with a system font stack or self-hosted fonts.

## Accuracy

Content is compiled from the official Carrera DIGITAL 124/132 Control Unit documentation. Wording and step order can vary slightly between firmware revisions. If something doesn't match your unit, the printed manual supplied with your set is the final authority.

Not affiliated with Carrera / Stadlbauer. All trademarks belong to their owners.

## License

MIT for the code. The instructional content is a paraphrased summary of publicly available product documentation.
