---
description: Generate print and eBook delivery checklists and a file package guide for publisher submission.
argument-hint: "[printer/publisher name and print run details, optional]"
---
# /deliver
Generate the complete delivery package guide for a finished book cover.

## Steps
1. **Print spec** — Apply the `print-delivery-spec` skill to generate the print delivery checklist: PDF/X-1a format, CMYK, 300 DPI, bleed, fonts, barcode, and preflight requirements.
2. **eBook spec** — Within `print-delivery-spec`, generate the separate eBook delivery checklist: JPEG/PNG, RGB/sRGB, platform-specific dimensions (Amazon KDP, IngramSpark, Apple Books, EPUB), and thumbnail legibility check.
3. **Typography check** — Cross-reference `cover-typography` spec to confirm all fonts are either outlined or properly licensed for embedding.
4. **Layout check** — Cross-reference `layout-composition` spec to confirm bleed, safe zones, and spine measurements are reflected in the final file.
5. **Asset package** — Produce a File Package Guide listing every file to include in the submission folder (print PDF, eBook JPEG, working file archive, font folder, image licenses, barcode EPS).

## Output
Submission-ready delivery package guide containing:
- Print delivery checklist (PDF/X-1a, CMYK, 300 DPI, all preflight items)
- eBook delivery checklist (per-platform specs and file requirements)
- Asset package manifest (every file required in the submission folder)
- Sign-off block for designer and publisher approval
