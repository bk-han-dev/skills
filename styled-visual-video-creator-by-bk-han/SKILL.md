---
name: Styled Visual Video Creator By BK Han
description: Use when a video needs a consistent visual style or on-screen slides/frames: code-drawn numbered styles, HTML frames from a design system, and motion handed to a video engine, all from one brief.
---
# Styled Visual Video Creator

Source: "Build Your Own Creative Agent Skills" (AICON 2026, 8 Oct 2026, *SCAPE, Singapore, Tianyu Xu; AIBLE framework by Danford Tan, Sange Nirahan, Tianyu Xu).
Principle: even the best AI team needs a director. Your idea, brief and direction decide the result. If the outcome is "the room understands this", slide software is one option, not the starting point.

## A. Deck as a folder (A + B x C = D)
1. A. Content + context first: get the production brief (5W1H, from idea-to-brief) before any layout.
2. B. Design system second, decided once: a token file for colours and type (typography tokens, colour palette) and a stylesheet with the layouts (CSS).
3. C. AI engine: the agent writes the slides as raw HTML content into that system.
4. D. Final product: render/export the deck (HTML, then PDF/PNG if needed). Check every slide visually before handing it over.
Folder: deck/tokens.(css|json), deck/styles.css, deck/content.html, deck/assets/.

## B. Programmable aesthetics (code-draw-styles)
1. Keep a numbered style library (e.g. 100 styles: watercolour, ukiyo-e, risograph, blueprint, pixel art, low poly, cyanotype, Bauhaus, synthwave/VHS).
2. Trigger when someone names a style number ("style 077") or asks to turn a photo or idea into a style.
3. Each style = constraint matrix (palette, primitives, grid) + parameters; draw with Python code, no image model required.
4. For motion (e.g. synthwave, frame-by-frame), hand frames or references to a video engine.
5. Prompt pattern: "/code-draw-styles CREATE <subject> in <style> ...".

## C. Headless pipelines (advanced)
Human references -> code generation (agent turns references into coordinates/scripts) -> headless execution (e.g. Blender with no GUI).

## Rules
- Draft only. Show outputs to the owner; nothing is published, sent or changed without approval.
- Confirmation lists: number each item, end with an "All" option.
- Use only facts from the brief; no invented stats.
