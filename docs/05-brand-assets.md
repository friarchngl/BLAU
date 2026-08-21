# BLAU — Brand assets & colour guideline

_Updated 2026-08-21 when the official logo files were supplied._

## Official colours

Sampled directly from the supplied logo PNGs (mean of fully-opaque pixels), so these are the
real values, not estimates.

| Token | Hex | Role |
|---|---|---|
| `--blau-navy` | `#133A6B` | **Primary.** The logo navy. |
| `--blau-cream` | `#F7F3EB` | **Secondary.** The logo cream — warm off-white, not pure white. |
| `--blau-navy-deep` | `#0C2445` | Derived. Site ground, dark enough to carry the cream logo. |
| `--blau-navy-mid` | `#1D4E86` | Derived. Hovers, rules, secondary fills. |

### Correction to the earlier guess

Before the logo files arrived I sampled colours off the 2025 menu PDF and had:
`#414889` (heading blue) and `#2D283D` (cover ground). **Neither is the brand navy.**
The real navy `#133A6B` is deeper and cooler, and the real light tone is a warm cream
`#F7F3EB`, not the near-white `#FDFDFD` I had. The site tokens have been corrected.

The menu values are kept in the stylesheet as `--menu-cover` and `--menu-heading` for
reference, but are no longer used to style anything.

**Still worth confirming:** whether `#414889` on the printed menu was a deliberate second
brand colour or a print/conversion drift from `#133A6B`. If there is a written brand guideline,
that would settle it.

## Files

Untouched originals live in `assets/brand-original/`. The web copies in
`site/assets/brand/` are the same artwork with fully-transparent margins trimmed off, so they
can be positioned by CSS without invisible padding.

| File | Size (trimmed) | Use |
|---|---|---|
| `blau-cream.png` | 1302 × 249 | Wordmark on dark grounds — header, hero |
| `blau-navy.png` | 1302 × 249 | Wordmark on light grounds |
| `eatery-coffee-cream.png` | 1302 × 53 | Sub-lockup on dark grounds |
| `eatery-coffee-navy.png` | 745 × 29 | Sub-lockup on light grounds |

Both cream files are 1302px wide, so setting them to the same CSS width stacks them into the
full lockup with the ends aligned. That is how the hero mark is built.

**Note on `eatery-coffee-navy.png`:** it was supplied at a different width (745px) to the other
three, so it will not stack cleanly against `blau-navy.png` without scaling. Worth requesting a
matched-width version.

## Still missing

- **Vector artwork** (SVG / AI / EPS). Everything here is raster, so the logo cannot scale
  cleanly for print, large screens, or a favicon. This is the single most useful thing to get next.
- **The brand typeface.** The site currently uses **Poppins** as a stand-in — closest free match
  to the geometric sans on the menu (single-storey `a`, rounded terminals). One variable swap
  once the real face is known.
- A horizontal / single-line lockup, if one exists.
- Any icon or monogram mark (the cut-through `A` would make a strong standalone device).
