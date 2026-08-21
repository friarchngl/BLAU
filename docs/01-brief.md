# BLAU — Website Project Brief

_Compiled 2026-08-21 from the 2025 menu PDF, Instagram, WhatsApp, and public listings._

## 1. The business

| | |
|---|---|
| **Brand name** | BLAU |
| **Full lockup** | BLAU EATERY & COFFEE |
| **Category** | All-day eatery + specialty coffee bar (fusion brunch / casual dining) |
| **Location** | Jl. Pelepah Elok I, QA2/7, Kelapa Gading, North Jakarta |
| **Hours** | Daily 10:00–22:00 |
| **Instagram** | [@blau.id](https://www.instagram.com/blau.id/) (secondary handle seen in listings: @blau.eatery) |
| **WhatsApp** | [+62 819 9971 8181](https://wa.me/6281999718181) |
| **Also listed** | +62 821-1723-5158 · blau.eatery@gmail.com · GoFood, Facebook `/blau.eatery` |
| **Domain** | Not yet supplied — **needs a decision** |

**Positioning in one line:** minimalist, cozy neighbourhood eatery in Kelapa Gading with a
punchy fusion menu and a serious coffee program.

**Signature items people search for:** Aglio Oglio Pork Belly, Balinese Pasta, Sambal Matah
rice bowls, Grilled Oxtail, Blau Signature coffee, Seasalt Latte.

## 2. What the menu tells us about the brand

- **Cuisine is deliberately cross-cultural** — Indonesian (nasi goreng, sambal matah, sate
  maranggi, oxtail), Japanese (katsudon, karaage, saikoro, izakaya), Thai (kana moo krob,
  thai tea), Korean (gochujang), Italian (pasta, pizza). The site copy should own this
  "one kitchen, many passports" idea rather than apologise for it.
- **Pork is on the menu and is a selling point** (pork belly, bagoge, salt & pepper pork,
  moo krob). This is a real differentiator in Jakarta and a filtering signal for the
  audience — worth being clear about, not hidden.
- **Coffee is a full program, not an afterthought** — 15 coffee SKUs including manual brew
  V60 with guest beans, cold brew, house-made sea salt foam. That deserves its own page.
- **Price band:** food mostly 35k–90k, a few hero items to 137k; drinks 12k–58k. Mid-market,
  everyday-repeat pricing. Not fine dining. The site should feel warm and accessible, not precious.
- **There is a Kids Meal section** → families are a real segment. Weekend brunch crowd.

## 3. Visual identity

_Colours below are the official values sampled from the supplied logo files — see `docs/05-brand-assets.md`._

| Token | Hex | Where it appears |
|---|---|---|
| `blau-navy` | `#133A6B` | **Official brand navy** (from logo files) |
| `blau-cream` | `#F7F3EB` | **Official brand cream** — warm off-white, not pure white |
| `blau-navy-deep` | `#0C2445` | Derived site ground |
| `menu-cover` | `#2D283D` | Menu cover ground — print only, not a brand colour |
| `menu-heading` | `#414889` | Menu section headings — print only, needs confirming |

- **Logo:** wordmark `BLAU`, all caps, wide-tracked geometric sans, with a **distinctive
  cut-through `A`** (the crossbar breaks the left stem). Reversed white on ink for the cover.
  Sub-lockup `EATERY & COFFEE` in small caps beneath, seen on cups and takeaway packaging.
- **Type on the menu:** a geometric/humanist sans throughout — headings are heavy weight with
  a single-storey `a` and rounded terminals (reads like Poppins / Futura-adjacent, closest
  free match: **Poppins** or **Outfit**); body is a lighter neutral grotesque (closest free
  match: **Inter** or **DM Sans**). *Needs confirmation from whoever made the menu.*
- **Photography direction:** two consistent setups — (a) top-down on textured white plaster,
  (b) dish on a deep-navy textured slab. Black ceramic ribbed plates. Warm natural light,
  no heavy filters. Branded greaseproof paper and wire fry baskets recur.
- **Layout habit worth carrying to the web:** big colour heading, generous white space, photo
  and text alternating across the spread — never a dense grid. That is already an
  editorial-web layout; the site should inherit it directly.

## 4. Assets on hand

| Asset | Path |
|---|---|
| Original menu PDF (12 pp) | `assets/BLAU-menu-2025.pdf` |
| Menu pages rendered to PNG | `assets/menu-pages/p001.png` … `p012.png` |
| Full menu transcription | `docs/02-menu.md` |
| Reference research | `docs/03-references.md` |
| Style directions | `docs/04-style-directions.md` |
| Brand assets & colour | `docs/05-brand-assets.md` |
| Official logo files | `assets/brand-original/` (untouched) · `site/assets/brand/` (trimmed for web) |
| Homepage build | `site/index.html` |

**Not yet supplied — will need to be gathered:**
- Vector logo (SVG/AI) — only raster PNGs so far — and the actual brand typeface
- Interior / atmosphere photography (only food shots exist so far)
- About story, team, opening history
- Google Maps embed link + exact coordinates
- Whether other outlets exist or are planned

## 5. Working assumptions for the site

Stated so they can be corrected rather than silently baked in:

1. **Goal priority:** (1) get people to walk in / order, (2) show the menu credibly,
   (3) look good enough to be the link in the Instagram bio. Not e-commerce.
2. **Primary CTA:** WhatsApp `wa.me/6281999718181` — reservations and enquiries. Secondary:
   Google Maps directions, and delivery via GoFood/GrabFood.
3. **Language:** English-first with Indonesian menu item names kept as-is, matching how the
   printed menu already reads. Bilingual toggle only if you want it.
4. **Scope:** single-location marketing site — Home, Menu, About, Visit/Contact. Menu is the
   heaviest page and should be real HTML (not a PDF embed) so it is searchable and mobile-friendly.
5. **Platform:** open. WordPress + Elementor if you want to edit prices yourself; a static
   build if you want it fast and are happy for me to make edits.

## 6. Open questions

- Do you own a domain yet? (`blau.id` is taken as an IG handle — is the `.id` domain free?)
- WordPress/Elementor, or a hand-built static site?
- Is the 2025 menu the *current* menu, or do prices need updating before launch?
- One outlet only, or is a second location coming?
- Do you want online ordering embedded, or just deep links out to GoFood/GrabFood?
