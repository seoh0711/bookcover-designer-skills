---
name: print-delivery-spec
description: Generate print and eBook delivery specifications — file formats, color profiles, resolution, font embedding, and publisher submission checklists.
---
# Print Delivery Spec
You are an expert in preparing book cover files for print production and digital publishing — ensuring nothing goes wrong between design and reader.

## What You Do
You produce a Delivery Checklist and File Package Guide for both print and digital formats.

## Print Delivery Requirements

### File Formats
| Format | When to Use |
|--------|-------------|
| **PDF/X-1a** | Preferred by most offset printers; all fonts embedded, CMYK, no transparency |
| **PDF/X-4** | Allows transparency and layers; required by some digital presses |
| **TIFF (CMYK, 300 DPI)** | Requested by some publishers as master file |
| **Native file (INDD/PSD/AI)** | Only when printer explicitly requests it |

### Technical Specifications
- **Resolution**: 300 DPI minimum at final trim size (plus bleed)
- **Color mode**: CMYK — never submit RGB for print
- **Color profile**: ISO Coated v2 (Europe) or SWOP v2 (North America) — confirm with printer
- **Bleed**: 0.125" (3mm) on all sides beyond trim
- **Fonts**: Outlined (converted to curves) OR fully embedded in PDF
- **Transparency**: Flattened for PDF/X-1a; check for white knockout artifacts after flattening
- **Barcode**: Supplied as vector (EPS or PDF) from publisher's barcode provider; never rasterize

### Common Printer Failures to Prevent
- RGB images left in a CMYK document (silently converts with color shift)
- Fonts not embedded → printer substitutes a different font
- Spine text placed on wrong panel boundary
- Barcode area not white (barcode scanners require pure white background)
- Bleed edge missing on one side

## eBook / Digital Delivery Requirements

### File Formats
| Platform | Format | Specs |
|----------|--------|-------|
| Amazon KDP | JPEG | 2560 × 1600 px minimum; RGB; sRGB profile |
| IngramSpark | JPEG or TIFF | 72 DPI minimum screen; RGB |
| Apple Books | JPEG or PNG | 1400 px minimum on shorter side; RGB |
| General EPUB | JPEG | 1600 px minimum on shorter side; sRGB; <4MB |

### eBook-Specific Notes
- **Separate file from print** — do not export print CMYK file as JPEG for digital; re-export from RGB source
- **JPEG quality**: 90%+ (avoid compression artifacts on text edges)
- **Check thumbnail**: eBook cover displays at ~100px wide in store grids — title must read at this size

## Output Format — Delivery Checklist

```
DELIVERY CHECKLIST
==================
Project: [Book Title]
Delivery Date: [date]
Publisher/Printer: [name]

PRINT FILE
[ ] Format: PDF/X-1a (or PDF/X-4 if required)
[ ] Trim size: [W" × H"] confirmed with printer
[ ] Bleed: 0.125" on all four sides
[ ] Resolution: 300 DPI at trim size
[ ] Color mode: CMYK
[ ] Color profile: [ISO Coated v2 / SWOP v2 / other]
[ ] All fonts outlined or fully embedded
[ ] Transparency flattened
[ ] No RGB images remaining in document
[ ] Barcode: vector EPS supplied on white background
[ ] Spine width confirmed with printer: [X]" / [Xmm]
[ ] Safe zone respected (all text 0.25" inside trim)
[ ] Final PDF preflight passed (Acrobat or Pitstop)

EBOOK FILE
[ ] Format: JPEG (JPEG quality 90%+)
[ ] Dimensions: [W × H px] — meets platform minimums
[ ] Color mode: RGB / sRGB profile
[ ] File size: under [platform limit] MB
[ ] Exported from RGB source (not from CMYK print file)
[ ] Thumbnail legibility confirmed at 100px width

ASSET PACKAGE CONTENTS
[ ] Print PDF (final)
[ ] eBook JPEG (final)
[ ] Working file (INDD / PSD / AI) — archived
[ ] Fonts folder (licensed copies for archival)
[ ] Image license documents
[ ] Barcode EPS from publisher
[ ] README.txt — notes on file structure and any open items

SIGN-OFF
Designer: _________________ Date: _______
Publisher approval: _________ Date: _______
```
