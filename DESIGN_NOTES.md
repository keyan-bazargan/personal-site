# Design Refresh — Analog / Tactile Direction

Working notes for the design refresh on branch `claude/design-refresh-animations-cmlrJ`.

## Context

The site currently runs Hugo + PaperMod with a single-page serif aesthetic (Cormorant Garamond italic), a cinematic hero image, and zero JavaScript. The goal of the refresh is to push further into an **analog / field-notebook** feel without losing the existing minimalism.

2026 design research points strongly toward "anti-AI crafting": tactile textures, hand-made imperfection, micro-delight animations, and a deliberate rejection of flat digital polish.

## Five directions considered

### 1. Paper & film-grain substrate
A subtle animated grain overlay (SVG turbulence or a looping noise PNG at ~4% opacity) across the whole page, plus a faint paper/vellum texture behind body copy. Makes the serif type feel letterpressed instead of screen-rendered. Very low JS cost.

### 2. Typewriter + ink-bleed intro
The home tagline types itself out on load, with a blinking caret and a faint "ink bleed" behind each glyph. One-shot only — doesn't repeat on scroll. Respects `prefers-reduced-motion`.

### 3. Analog cursor
Replace the pointer with a small crosshair/reticle (darkroom loupe or astronomical finder — fitting given *Moon Shot*). Magnetic pull toward links; spotlight-reveal mode over the hero image. Biggest "wow" for the least code.

### 4. Hand-drawn marginalia & dividers
Swap `---` separators for SVG sketched lines / asterisms. Underline links with a hand-drawn wobble instead of a straight rule. Book list gets little hand-drawn check-bullets.

### 5. Tactile page transitions
Crossfade-to-black with a subtle film-leader "countdown" flash between routes, or a page-turn curl for writing posts. More ambitious — worth it only if we want writing to feel like a zine.

## Recommendation

Start with **#1 + #3 + #4**. They're additive, stack cleanly on top of PaperMod, and collectively shift the feel from "clean blog" to "analog field notebook" without a framework swap.

- **#2** is a nice add-on for the home page only.
- **#5** stays on hold unless we want the site to feel noticeably heavier.

## Decision

Going with the recommendation: **#1 (grain + paper), #3 (analog cursor), #4 (hand-drawn marginalia)**.

## Sources

- [Texture, warmth and tactile rebellion — Creative Bloq](https://www.creativebloq.com/design/graphic-design/texture-warmth-and-tactile-rebellion-the-big-graphic-design-trends-for-2026)
- [Digital Harmony: Embracing Analog in Modern Web Design — Squarespace](https://pros.squarespace.com/blog/analog-design-trend)
- [Custom Cursor Effects — Codrops](https://tympanus.net/codrops/2019/01/31/custom-cursor-effects/)
- [Hovers, Cursors and Cute Interactions — Awwwards](https://www.awwwards.com/awwwards/collections/hovers-cursors-and-cute-interactions/)
- [Retro collection — Awwwards](https://www.awwwards.com/awwwards/collections/retro/)
- [11 Motion Design Trends for 2026 — Envato](https://elements.envato.com/learn/motion-design-trends)
