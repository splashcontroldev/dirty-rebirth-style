# Dirty Rebirth style guide

> **v0.5.0 · provisional.** Stylised realism in evacuated London, told through street graffiti.

![palette](swatches.png)

Painted, not photographed. Between realistic and cartoony, like Dirty Bomb. Overcast cool daylight, wet streets, Victorian brick railway arches, layered resistance graffiti (red and black stencils, tags, colourful throw-ups), clean white-and-yellow quarantine barriers, and red poppies growing through the cracks.

Free to use for your own projects (MIT). If you have an AI assistant, point it at this repo: it reads
[`AGENTS.md`](AGENTS.md) and applies the style for you.

## Use it
**Any website:** copy [`tokens/dr.css`](tokens/dr.css) in, then use the variables:
```css
body   { background: var(--dr-asphalt); color: var(--dr-paper); font-family: var(--dr-font-body); }
h1, h2 { font-family: var(--dr-font-display); text-transform: uppercase; }
.cta   { background: var(--dr-spray-red); color: var(--dr-paper); border-radius: var(--dr-radius); }
```
Also here: [SCSS](tokens/dr.scss) · [Tailwind preset](tokens/tailwind.preset.js) · [W3C design tokens JSON](tokens/dr.tokens.json) (Style Dictionary, Figma Tokens Studio).

**Always get the latest:** `https://raw.githubusercontent.com/splashcontroldev/dirty-rebirth-style/main/tokens/dr.css`

## Colours
| Token | Hex | Use |
|---|---|---|
| `--dr-spray-red` | `#a10d0c` | Brand accent. The one call to action per screen. Measured from the graffiti red in the key art. |
| `--dr-poppy-red` | `#c8231e` | Lighter accent for hover/highlight on red elements. |
| `--dr-sky` | `#8093a0` | Cool neutral: secondary text, borders, quiet surfaces. |
| `--dr-brick` | `#5a4d3e` | Warm neutral: panels, cards, dividers. |
| `--dr-paper` | `#cdd0d4` | Primary text on dark; paper/poster surfaces. |
| `--dr-muted` | `#c4c1ba` | The DIMMEST text allowed: secondary values, captions, the legal line. Passes 4.5:1 as rendered on calm dark paper at every window size (check-text-legibility.py; #b3b0a8 read 4.5:1 at 1100x720, too close). Never lower text contrast with opacity - use this. |
| `--dr-asphalt` | `#151616` | Page background. |
| `--dr-asphalt-2` | `#1f2123` | Raised surface on the page background. |
| `--dr-teal` | `#407a7c` | Rare secondary accent (graffiti throw-ups). Use sparingly. |
| `--dr-hazard` | `#e8c33a` | World colour for quarantine barriers and warnings ONLY - never a button or brand colour. |

## Type
- **DirtyBomb NX Black** (display): Headings, button words, labels. The Dirty Bomb voice. [Google Fonts](Splash Damage's own Dirty Bomb display face (Process Type Foundry licence, held by SD). Read from the player's installed game by the launcher and client; NEVER bundled or served. Public sites fall back to Big Shoulders Stencil Display (OFL).)
- **Rubik Spray Paint** (spray): Graffiti accents only (a word or two). Never body text. [Google Fonts](https://fonts.google.com/specimen/Rubik+Spray+Paint)
- **Exo 2** (body): Body text and UI. Dirty Bomb's own UI font (SIL OFL, safe to bundle and serve). Replaces Inter, the #1 'looks AI-made' tell. [Google Fonts](https://fonts.google.com/specimen/Exo+2)
- **Big Shoulders Stencil Display** (display-public): Public web fallback for the display face only. [Google Fonts](https://fonts.google.com/specimen/Big+Shoulders+Stencil+Display)

## Rules
- QUIET buttons (account, verify, settings actions) are 40px tall. The WALL pieces - tab strips and the call-to-action sticker on the home screen - are painted paper sized by the approved style frame (launcher r4), not by the button height. Owner approved that frame on 2026-09-22.
- One red ACTION per screen: the call to action, plus (only while it is pointing at it) the CLICK THIS hint. Tab markers, toggles, radios and hover edges are paper, not red.
- Text stays generous (16px body minimum). Paragraphs are 20 words or fewer. No em dashes in UI copy.
- Buttons carry words, not stock icons or decorative chevrons.
- Textures over flat fills: paper, brick, spray overspray and drips, tape, torn poster edges.
- Texture never sits behind letters. Every word printed on paper gets a calm wash in that paper's own colour (surface.calm-*), and every text element must pass the legibility check (contrast and background noise, measured on screen).
- Nothing perfectly symmetrical: panels rest slightly off-angle, the home card bleeds off the edge.
- Motion feels physical (paper settling, paint spraying, rain), never glowing or bouncy. See motion.banned.
- Corners are nearly square (2px). Nothing pill-shaped.

## Avoid
- Neon glows, decorative frosted-glass cards, soft purple/blue gradients - the generic AI look. (Smoke over OUR painted art is allowed: it shows the street, it does not decorate.)
- Sunsets or orange skies, glossy plastic, over-sharpened photo/HDR looks.
- Radiation trefoil symbols and generic military props.
- Hazard yellow as a brand or button colour, and moving hazard stripes anywhere.
- Stock thin-line icons on buttons; oversized buttons; paragraphs that explain what a button already says.

## Changes
See [CHANGELOG.md](CHANGELOG.md). This repo is generated automatically from Dirty Rebirth's own design tokens,
so it updates whenever the game's look changes.

---
*Dirty Bomb is © Splash Damage. This guide covers Dirty Rebirth's own look only and contains no Splash Damage artwork.*
