---
description: Analyze a book brief and generate three distinct cover concept directions with visual keywords, mood, and market context.
argument-hint: "[book title, genre, and target audience]"
---
# /conceptualize
Generate three cover concept directions from a book brief.

## Steps
1. **Collect the brief** — Gather title, genre, target audience, and core message. If any are missing, ask before proceeding.
2. **Analyze** — Apply the `book-concept-analysis` skill to extract visual keywords, mood adjectives, and a primary image archetype.
3. **Benchmark** — Apply the `genre-benchmark` skill to identify dominant cover patterns, saturated clichés, and differentiation opportunities in this genre.
4. **Develop concepts** — Apply the `visual-storytelling` skill to generate three concept directions (Safe / Balanced / Bold), each with a distinct storytelling device and eye-path logic.
5. **Present** — Output the full Concept Brief with all three directions, benchmark context, and a recommended direction with rationale.

## Output
Three-option Concept Brief containing:
- Visual keywords and mood adjectives
- Genre benchmark summary (what's saturated, what's open)
- Direction A (Safe), B (Balanced), C (Bold) — each with visual premise, storytelling device, and reference covers
- Recommended direction with strategic rationale

Consider following up with `/book-cover-design:design-system` to build the typography, color, and layout system for the chosen direction.
