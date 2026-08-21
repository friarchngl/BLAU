# BLAU — Reference Set

_Compiled 2026-08-21. Sites marked **✔ inspected** were fetched and read for this doc.
Sites marked **○ candidate** come from search and my own knowledge — worth opening together
before we commit, but I have not verified their current state._

---

## 0. Read this first: what the two you picked have in common

You sent **Locavore NXT** and **ISMAYA**. They are very different businesses, but both are
doing the same thing that BLAU's printed menu already does:

> **Lead with a point of view, let photography carry the weight, and keep the typography quiet.**

Neither site is a "restaurant template". Neither opens with a stock hero of a smiling table.
Both treat the brand as an editorial subject.

The important caveat: **both are the wrong *scale* for BLAU.** Locavore NXT is a destination
tasting-menu venue where people plan a trip; ISMAYA is a 20-brand group portfolio site. BLAU
is one neighbourhood eatery where the winning action is "walk in on Saturday" or "order on
GoFood". So we take their **tone and restraint**, but not their **information architecture** —
BLAU's site has to be faster to act on.

---

## 1. The two you gave

### ✔ Locavore NXT — [locavorenxt.com](https://locavorenxt.com/)
Ubud, Bali. Hyper-local tasting-menu restaurant, "a localised rebellion."

| | |
|---|---|
| **Structure** | Tasting Menu · Features · Collaborators · Events & Programs · Visit. Sister venues (Nusantara, Night Rooster) each get their own booking path. |
| **Design** | Minimalist, monochrome logo, clean modern type, nature-led full-bleed imagery, generous air. |
| **Standout** | An **interactive multi-floor plan** — tunnel, ground, first, second, lower-ground — that lets you explore the building before visiting. A "What's On?" board runs events out to 2026. Booking hands off to RevAsi. |
| **What BLAU should steal** | Progressive disclosure — sections that expand instead of dumping everything at once. And the idea that **the space itself is content**. BLAU has a room; nobody has photographed it yet. |
| **What BLAU should not copy** | The whole reservation-first architecture. BLAU is walk-in. |

### ✔ ISMAYA — [ismaya.com](https://www.ismaya.com/)
Indonesian lifestyle/hospitality group. "Creating the Good Life."

| | |
|---|---|
| **Structure** | Brands sorted into five **pillars** — Elevate, Unite, Ignite, Everyday, Wellbeing — rather than an A–Z list. Plus Catering, ISMAYA LIVE, ISMAYA+ membership, news, careers. |
| **Design** | Dark/neutral grounds, monochrome logo, strong type hierarchy, **video backgrounds in section headers**, high-quality venue photography. |
| **Standout** | Categorising by *mood and occasion* instead of by cuisine. That is a genuinely good idea and it scales down. |
| **What BLAU should steal** | The pillar idea, applied to the menu: BLAU's menu is a mess of cuisines if you list it flat, but it is coherent if you sort it by **occasion** — *Quick lunch · Long brunch · Coffee & work · Feed the family*. Also: video in the hero. |
| **What BLAU should not copy** | Group-portfolio depth. One venue, one story. |

---

## 2. Closest peers — Indonesian F&B, same market, same customer

These matter most. They set the expectation your actual customers already have.

### ✔ Common Grounds — [commongrounds.co.id](https://commongrounds.co.id/)
Jakarta specialty roastery + café group.
- **Nav:** Home · Menteng Tennis Club · About · Cafés · Shop · Roastery · Archive · Career.
- Minimalist dark logo, neutral premium palette, mobile-first collapsible nav, persistent cart.
- **Take:** the **Roastery** and **Archive** pages. They prove a coffee program is real by
  giving it its own room. BLAU has V60 with rotating guest beans and house-made sea salt foam —
  that deserves the same treatment instead of being 15 rows in a price list.
- **Also take:** splitting "Cafés" (visit) from "Shop" (buy) as two separate top-level intents.

### ✔ Kopi Kenangan — [kopikenangan.com](https://www.kopikenangan.com/)
Mass-market Indonesian coffee chain — the *opposite* end from Locavore, and useful for that.
- White grounds, dark text, modern sans, heavy app-download push, themed drink "series"
  (Dreamy Choco Series, IP collabs), outlet finder with Google Maps, WhatsApp consumer service.
- **Take:** the **seasonal/themed drink collection** pattern — a merchandising slot that gives
  you a reason to update the site monthly. Also their WhatsApp-as-support convention, which is
  exactly right for Indonesia and matches BLAU's `wa.me` link.
- **Do not take:** the app-first architecture or the density. BLAU has no app.

### ○ 1/15 Coffee — `satuperlimabelas.com`
Scandinavian-inspired Jakarta chain, the coffee-professional's choice, in-house roasting.
- **Why it's here:** closest visual cousin to BLAU's actual palette — cool, restrained, clean
  lines, soft light. Worth opening as a direct "could BLAU look like this?" test.

### ○ Kopi Kalyan — `kopikalyan.com`
Jakarta, vintage-eclectic interior, own roasting, food alongside coffee. The Cikajang flagship
(Kopi Kalyan Archive) is a two-storey space with a cold brew bar.
- **Why it's here:** the closest *business model* match to BLAU — coffee **and** a real food
  menu, neighbourhood-scale, warm rather than clinical.

### ○ Anomali Coffee — `anomalicoffee.com`
Since 2007, the standard-bearer for Indonesian single-origin.
- **Why it's here:** for how to talk about beans and origin credibly in an Indonesian context
  without sounding like a translated Scandinavian brand.

### ○ Tanamera Coffee — `tanameracoffee.com`
Jakarta roaster with a strong award/provenance story.
- **Why it's here:** provenance storytelling that stays readable.

---

## 3. All-day eatery + strong brand — the format BLAU actually is

### ✔ Dishoom — [dishoom.com](https://www.dishoom.com/)
**The single most useful reference in this list.** Bombay-café-inspired all-day restaurant group,
Awwwards/Webby/James Beard winner.
- **Nav:** Explore · Cafés · Menus · Shop · Stay, with **"Book a table" as a persistent sticky CTA**.
- **Menus split by meal period** — Breakfast, All Day, Drinks, Puddings, plus Group Feasts and
  Vegan cuts. Each menu is its own `/menu/…` route (good for SEO, shareable, printable).
- Warm, photograph-dominant, culturally specific. The story section is genuinely worth reading —
  each location has its own founding myth set in a different moment of Indian history.
- Card system reused consistently for recipes, locations, products. Newsletter mid-page and in footer.
- **What BLAU should steal, concretely:**
  1. **Menus as separate routed pages, cut by how people eat** — not one PDF, not one endless scroll.
     For BLAU: *Rice Bowls · Pasta & Pizza · Small Plates · Coffee · Cold Drinks*.
  2. **The persistent CTA.** BLAU's is WhatsApp, not booking, but the pattern is identical.
  3. **Cultural specificity as the brand voice.** Dishoom sells Bombay. BLAU can sell the
     genuinely unusual thing on its menu: sambal matah next to carbonara next to gochujang,
     and pork done properly in Kelapa Gading. That is a story; "cozy minimalist cafe" is not.

### ○ Ottolenghi — `ottolenghi.co.uk`
Deli-restaurant-cookbook brand. Look at how food photography and a distinct colour system carry
the whole identity with almost no decoration.

### ○ Bluestone Lane — `bluestonelane.com`
Australian-style all-day café at scale. Look at their location/hours pattern and how they make
"coffee shop" and "restaurant" coexist without the site splitting in half.

### ○ Sunday in Brooklyn — `sundayinbrooklyn.com`
Brunch-led all-day restaurant. Warm, photographic, small — closest in scale to a single BLAU outlet.

---

## 4. Editorial restraint — for typography and pacing only

### ○ Noma — `noma.dk`
Clean editorial layout, immersive full-bleed photography, refined type, whitespace used to
signal luxury. Famous for letting the food photography do all the work.
- **Take:** pacing and whitespace discipline. **Do not take** the exclusivity — BLAU is a
  neighbourhood place, and Noma's coldness would read as unfriendly at 60k a bowl.

### ○ Atomix — `atomixnyc.com`
Two-Michelin-star, elegant **single-page** design, muted tones, generous whitespace.
- **Take:** proof that a single well-paced page can carry a whole restaurant. If BLAU wants a
  small site fast, this is the shape.

---

## 5. Where the 2026 field is going

From current design-press roundups, restaurant web design has split into two camps:

1. **Fine dining → editorial restraint.** Typography *is* the branding; the typeface alone
   signals the positioning.
2. **Fast-casual → custom type and illustration systems** to escape category defaults.

Practical requirements now treated as table stakes: fast load, clean type, mobile-first,
interactive/booking integrations.

**Where BLAU sits:** camp 2, borrowing camp 1's restraint. BLAU already owns an unusual asset —
that cut-through `A` in the wordmark and the `#414889` indigo. Nobody else in Jakarta casual
dining is using an indigo-forward palette; most default to warm brown/cream "cozy cafe". Leaning
into the blue is the single cheapest way to look like nobody else.

---

## 6. Shortlist — my recommendation

If you only open five before we start:

| Site | Open it for |
|---|---|
| **Dishoom** | Site architecture. This is the model. |
| **ISMAYA** | Sorting the menu by occasion, and hero video. |
| **Common Grounds** | How to give the coffee program its own room. |
| **Locavore NXT** | Restraint, and the idea that the space is content. |
| **Kopi Kenangan** | The Indonesian conventions: WhatsApp, outlet finder, seasonal drink drops. |

**The synthesis I would propose for BLAU:**
> Dishoom's architecture, at Atomix's size, in ISMAYA's tone, with Locavore's whitespace —
> rendered in BLAU's own indigo instead of the beige everyone else uses.

---

## 7. What I still need from you

1. **Any sites you actively dislike.** Faster to calibrate than more likes.
2. **Do you want the site to feel closer to Locavore (quiet, considered, slow) or to Dishoom
   (warm, busy, appetising)?** Both are defensible; they produce very different sites.
3. Whether hero **video** is possible — do you have any footage of the room or the bar?
4. Interior photography. Every reference above leans on it and BLAU currently has none.

## Sources

- [locavorenxt.com](https://locavorenxt.com/) · [ismaya.com](https://www.ismaya.com/) · [dishoom.com](https://www.dishoom.com/) · [commongrounds.co.id](https://commongrounds.co.id/) · [kopikenangan.com](https://www.kopikenangan.com/)
- [BLAU Eatery & Coffee on Instagram](https://www.instagram.com/blau.id/?hl=en) · [Facebook](https://www.facebook.com/blau.eatery/) · [GoFood](https://gofood.co.id/en/jakarta/restaurant/blau-eatery-coffee-41353093-a30a-4326-bda5-1f50cb8c7658)
- [Best restaurant websites of 2026 — StartDesigns](https://www.startdesigns.com/blog/best-restaurant-websites/) · [Best restaurant website designs — Colorlib](https://colorlib.com/wp/restaurant-website-designs/) · [29 best restaurant websites — Sage](https://sage.agency/industry/best-restaurant-websites-design/)
- [11 top specialty coffee shops and roasters in Jakarta — The Way To Coffee](https://www.thewaytocoffee.com/jakarta/) · [Jakarta specialty coffee guide 2025 — FLTR Magazine](https://fltrmagazine.com/2025/05/13/jakarta-specialty-coffee-guide-2025/) · [Trendiest coffee shops in Jakarta — What's New Indonesia](https://whatsnewindonesia.com/jakarta/ultimate-guide/trendiest-coffee-shops-jakarta)
