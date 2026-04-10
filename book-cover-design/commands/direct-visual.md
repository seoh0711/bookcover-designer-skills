---
description: Choose the right visual medium (photo, illustration, or AI) and produce a detailed brief for the creator or AI image tool.
argument-hint: "[concept direction and Design System, or book title]"
---
# /direct-visual
Create a Visual Direction Brief for the hero image or illustration on a book cover.

## Steps
1. **Extract the core visual** — From the Storytelling Concept Sheet (or re-apply `visual-storytelling` if needed), identify the primary visual element and its narrative role.
2. **Select the medium** — Apply the `image-illustration-direction` skill to evaluate photography vs. illustration vs. AI-generated image, make a recommendation with rationale, and complete the licensing checklist.
3. **Apply color direction** — Cross-reference `color-mood-system` output to ensure the image brief aligns with the palette (dominant tones, mood, atmosphere).
4. **Write the brief** — Produce the full Visual Direction Brief including subject description, style references, mood direction, and — if AI-generated — a structured, ready-to-paste prompt for Midjourney, DALL-E, or Stable Diffusion.
5. **Specify delivery** — Include technical delivery specs (format, resolution, color mode) for the creator or export settings.

## Output
Visual Direction Brief containing:
- Medium recommendation with rationale and licensing notes
- Subject / scene description (what to include, what to exclude)
- Style references and tonal benchmarks
- AI image prompt (if applicable) — formatted for direct use
- Delivery specs (format, DPI, color mode)

Consider following up with `/book-cover-design:deliver` to generate the print and eBook delivery package.
