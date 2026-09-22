# Instructions for AI assistants: apply the Dirty Rebirth style (v0.1.1)

You are styling a project in the **Dirty Rebirth** look. Stylised realism in evacuated London, told through street graffiti. Painted, not photographed. Between realistic and cartoony, like Dirty Bomb. Overcast cool daylight, wet streets, Victorian brick railway arches, layered resistance graffiti (red and black stencils, tags, colourful throw-ups), clean white-and-yellow quarantine barriers, and red poppies growing through the cracks.

## Do this
1. Import `tokens/dr.css` (or the SCSS / Tailwind / JSON file matching the project's stack). Never hard-code
   the hex values; always use the tokens so the project updates when this repo does.
2. Background `--dr-asphalt`, text `--dr-paper`, headings in the display font, uppercase.
3. Exactly one `--dr-spray-red` element per screen: the main call to action.
4. Give surfaces texture (paper grain, torn edges, spray drips) instead of flat fills or glows.

## Colours
- `#a10d0c` **spray-red**: Brand accent. The one call to action per screen. Measured from the graffiti red in the key art.
- `#c8231e` **poppy-red**: Lighter accent for hover/highlight on red elements.
- `#8093a0` **sky**: Cool neutral: secondary text, borders, quiet surfaces.
- `#5a4d3e` **brick**: Warm neutral: panels, cards, dividers.
- `#cdd0d4` **paper**: Primary text on dark; paper/poster surfaces.
- `#151616` **asphalt**: Page background.
- `#1f2123` **asphalt-2**: Raised surface on the page background.
- `#407a7c` **teal**: Rare secondary accent (graffiti throw-ups). Use sparingly.
- `#e8c33a` **hazard**: World colour for quarantine barriers and warnings ONLY - never a button or brand colour.

## Fonts
- display: Big Shoulders Stencil Display (https://fonts.google.com/specimen/Big+Shoulders+Stencil+Display), fallback Impact, 'Arial Narrow', sans-serif. Headings, labels, buttons. Stencil lettering like the stencils on the wall.
- spray: Rubik Spray Paint (https://fonts.google.com/specimen/Rubik+Spray+Paint), fallback 'Big Shoulders Stencil Display', sans-serif. Graffiti accents only (a word or two). Never body text.
- body: Inter (https://fonts.google.com/specimen/Inter), fallback 'Segoe UI', Roboto, Arial, sans-serif. Body text and UI copy. Provisional choice.

## Sizes
text-sm 14px, text-md 16px, text-lg 20px, text-xl 28px, text-2xl 40px, space-1 4px, space-2 8px, space-3 12px, space-4 16px, space-6 24px, space-8 32px, radius 2px, button-height 40px

## Rules
- Buttons stay modest in size; text stays generous (16px body minimum). Short sentences, short paragraphs.
- One red thing per screen: the call to action. Everything else is neutral.
- Textures over flat fills: paper, brick, spray overspray and drips, tape, torn poster edges.
- Every surface has a little life: subtle paper grain, a paint drip, a torn edge. Nothing perfectly flat and nothing perfectly symmetrical.
- Motion feels physical (paper settling, paint spraying), never glowing or bouncy.
- Corners are nearly square (2px). Nothing pill-shaped.

## Never
- Neon glows, glassmorphism, soft purple/blue gradients - the generic AI look.
- Sunsets or orange skies, glossy plastic, over-sharpened photo/HDR looks.
- Radiation trefoil symbols and generic military props.
- Hazard yellow as a brand or button colour.

## Generating images in this style
Prompt: Painted video-game concept art, stylised realism (between realistic and cartoony, hand-painted with broad confident brushwork, no photo look, no HDR). Evacuated near-future London under quarantine: overcast cool daylight, teal-grey sky, wet streets, Victorian brick railway arches, black cast-iron lamp posts and bollards, layered resistance graffiti (red and black spray stencils, tags, colourful throw-ups), clean white-and-yellow angular quarantine barriers, red poppies growing through cracks. Accents: spray red and poppy red; everything else cool and muted.
Negative prompt: neon, sunset, orange sky, glossy plastic, HDR, over-sharpened, photo-realistic, logos, watermark, readable text, radiation symbols
