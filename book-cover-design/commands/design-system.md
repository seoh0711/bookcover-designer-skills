---
description: Build the typography, color palette, and layout grid system for a chosen book cover concept direction.
argument-hint: "[chosen concept direction or Concept Brief]"
---
# /design-system
Build the complete design system for a book cover from a chosen concept direction.

## Steps
1. **Confirm the concept** — Take the chosen direction from the Concept Brief (or run `/book-cover-design:conceptualize` first if not yet done).
2. **Typography** — Apply the `cover-typography` skill to select genre-appropriate typefaces, define the four-tier hierarchy (title / subtitle / author / series), specify weight and tracking, and output a Typography Spec Sheet.
3. **Color** — Apply the `color-mood-system` skill to build a 3-color palette with psychological rationale, HEX/RGB/CMYK values, print warnings, and thumbnail contrast checks.
4. **Layout** — Apply the `layout-composition` skill to define the three-panel grid (front / spine / back), set bleed and safe zones, and produce a Layout Guide with compositional structure.
5. **Document** — Compile all three specs into a unified Design System document that a designer can work from directly.

## Output
Cover Design System document containing:
- Typography Spec Sheet (typefaces, weights, hierarchy, free alternatives)
- Color Palette Spec (background, primary accent, secondary accent — HEX/CMYK/RGB + print notes)
- Layout Guide (trim size, grid, bleed, safe zone, spine rules, back cover zones)

Consider following up with `/book-cover-design:direct-visual` to brief the image or illustration.
