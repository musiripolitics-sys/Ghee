# SATVA — complete asset manifest

> **Status: all 27 photograph slots are filled.** The files live in `assets/`
> as WebP, ~3 MB in total. Three open items are listed under *Known issues*
> at the foot of this file.


Everything the website needs, in four groups:

| Group | Count | Who supplies it |
|---|---|---|
| **A. Photographs** | 27 | Photographer / brand |
| **B. Logo & brand files** | 7 | Designer |
| **C. Icons** | 6 | Already drawn in SVG — supply only if you want custom |
| **D. Kolam & pattern art** | 8 | Already drawn in SVG — supply only if you want your own |

Groups C and D are **already built and working**. They are listed so you know
what exists and can replace any of it with your own artwork. Nothing in the
site is waiting on them.

The only things actually blocking launch are **Group A** and **Group B**.

---

# A. PHOTOGRAPHS — 27 frames

**Weighting.** Of the 27 frames, **9 are cows and farm**, **8 are ghee and
process**, **3 are food**, **3 are the product jars**, and **4 are people and
place. That is deliberate: the cow, the farm and the making of the ghee carry
the authenticity, and the jars are the smallest part of the story.

### Technical spec — applies to every photograph

| | |
|---|---|
| **Format** | WebP, quality 80–82. JPEG q80 is an acceptable substitute. |
| **Colour** | sRGB only. Adobe RGB desaturates in browsers. |
| **Metadata** | Strip EXIF except copyright. Bake in rotation. |
| **Naming** | Lowercase hyphenated, as given in the tables: `cow-grazing.webp`. |
| **Folder** | `assets/` |
| **Never** | Upscale. A sharp 1000px file beats a soft 2000px one. |

Weight targets: full-bleed ≤ 500 KB · editorial ≤ 300 KB · grid tiles ≤ 180 KB ·
small tiles ≤ 120 KB. Whole page under 4 MB with all 27 in place.

---

## A1. Cows and farm — 9 frames

The heart of the site. Shoot these in one session, same light, so they read as
one body of work.

| File | Shot | Ratio | Size |
|---|---|---|---|
| `hero-cow.webp` | **HERO.** A native Indian cow standing naturally on a Tamil Nadu farm. Tiled-roof house, coconut and banana trees, brass milk vessel, green pasture, early-morning light. | 4 : 4.6 | 1200 × 1380 |
| `cow-grazing.webp` | Cow grazing in open pasture, full body, rural Tamil Nadu | 16 : 11 | 1400 × 960 |
| `cow-and-calf.webp` | Cow with her calf, close and unposed | 4 : 3.45 | 1000 × 865 |
| `farmer-cattle.webp` | Farmer feeding, washing or leading the cattle — hands visible | 1 : 1 | 800 × 800 |
| `traditional-milking.webp` | Hand milking into a brass or steel pail | 1 : 1 | 800 × 800 |
| `farm-landscape.webp` | Wide farm landscape, coconut and banana trees, red soil | 1 : 1 | 800 × 800 |
| `story-farm.webp` | The farm in context — sheds, fodder, working daylight | 4 : 3.3 | 800 × 660 |
| `morning-scene.webp` | Kolam being drawn at the doorstep, tulasi maadam, brass vessel, **a cow in frame**, sunrise through coconut trees | 4 : 4.4 | 1200 × 1320 |
| `household-band.webp` | **FULL-BLEED.** Traditional home — woman in saree at a wooden churner, brass vessels, banana leaves, tiled roof | 16 : 9 | 2400 × 1400 |

**Hero note:** it renders upright on desktop and crops to **4 : 3.2 landscape on
phones**. Keep the cow centred with headroom top and bottom so both crops hold.

**Full-bleed note:** a dark gradient with the headline sits over the
**bottom-left third**. Keep that area quiet; put the action upper or right.

---

## A2. Ghee and the process — 8 frames

Six of these are new — the process timeline now has a photograph above every
step. They run in a row at small size, so each must read instantly as **one
clear object, centred, plain background**. Treat them as a matched set: same
surface, same light, same distance. Shot in sequence during one actual batch,
they double as proof the process is real.

| File | Step | Shot | Ratio | Size |
|---|---|---|---|---|
| `step-1-milk.webp` | 01 Milk | Fresh cow's milk in a brass vessel, surface still moving | 1 : 1 | 600 × 600 |
| `step-2-curd.webp` | 02 Curd | Set curd in an earthen pot, the surface just broken | 1 : 1 | 600 × 600 |
| `step-3-churning.webp` | 03 Churning | A wooden mathu mid-churn, hands on the rope | 1 : 1 | 600 × 600 |
| `step-4-butter.webp` | 04 Butter | Fresh white butter gathered, texture visible | 1 : 1 | 600 × 600 |
| `step-5-heating.webp` | 05 Slow heating | Butter melting in a heavy vessel over low flame | 1 : 1 | 600 × 600 |
| `step-6-ghee.webp` | 06 Golden ghee | Clear golden ghee being strained or poured | 1 : 1 | 600 × 600 |
| `signature-product.webp` | — | **THE GHEE SHOT.** Jar open, brass spoon lifting golden ghee, warm directional light, **granularity clearly visible** | 1 : 1.16 | 1200 × 1392 |
| `ghee-pour.webp` | — | Ghee being spooned over hot ven pongal on a banana leaf, caught while still moving. Steam welcome. | 4 : 4.2 | 1300 × 1365 |

`signature-product.webp` is the single most important frame after the hero.
The granular texture from traditional churning **is** the product's argument —
get in close enough that it is unmistakable.

---

## A3. Food — 3 frames

Homemade, not catalogue-plated. Banana leaves and brass serving vessels. Food
that looks cooked and eaten from.

| File | Shot | Ratio | Size |
|---|---|---|---|
| `food-pongal.webp` | *(this is `ghee-pour.webp` above — it serves both sections)* | 4 : 4.2 | 1300 × 1365 |
| `food-paruppu-sadam.webp` | Paruppu sadam with a spoon of ghee, brass vessel | 16 : 9 | 1100 × 620 |
| `food-payasam.webp` | Sakkarai pongal or payasam, served traditionally | 16 : 9 | 1100 × 620 |

`food-pongal.webp` crops to **4 : 3.4 on phones** — leave room top and bottom.

---

## A4. Product jars — 3 frames

| File | Shot | Ratio | Size |
|---|---|---|---|
| `product-250ml.webp` | 250 ml jar | 1 : 1.12 | 1200 × 1344 |
| `product-500ml.webp` | 500 ml jar | 1 : 1.12 | 1200 × 1344 |
| `product-1l.webp` | 1 litre jar | 1 : 1.12 | 1200 × 1344 |

**Shoot all three identically** — same angle, light, distance, label level and
facing front. They sit side by side and any drift is immediately visible.

If you can also supply them **cut out on transparent PNG**, they will sit
directly on the page's cream panels and look cleaner. Send both if easy.

---

## A5. Botanicals, kitchen and people — 4 frames

| File | Shot | Ratio | Size |
|---|---|---|---|
| `botanical-moringa.webp` | Fresh moringa leaves, close, natural light | 1 : 1 | 800 × 800 |
| `botanical-cumin.webp` | Cumin seeds, close, natural light | 1 : 1 | 800 × 800 |
| `kitchen.webp` | Traditional South Indian kitchen — brass vessels, stone or red-oxide floor, light through a wooden window | 4 : 4.7 | 1200 × 1410 |
| `story-family.webp` | The real people behind SATVA, if they are willing | 4 : 3.3 | 800 × 660 |
| `story-product.webp` | The jar in a traditional setting — kitchen shelf, banana leaf, brass tray | 4 : 3.3 | 800 × 660 |

Match the light between the two botanicals; they sit side by side.

A genuine photograph of the family does more for trust than any stock frame.

---

# B. LOGO AND BRAND FILES — 7 files

| File | Format | Spec | Used for |
|---|---|---|---|
| `logo.svg` | SVG | Full lockup, mark + wordmark, dark version | Header on cream |
| `logo-light.svg` | SVG | Same lockup in off-white / gold | Footer on green |
| `logo-mark.svg` | SVG | The gold knot mark alone, square | Favicon source, social, small uses |
| `logo.png` | PNG | Transparent, 400 px tall minimum | Fallback if SVG unavailable |
| `favicon.ico` | ICO | 32 × 32 and 16 × 16 in one file | Browser tab |
| `apple-touch-icon.png` | PNG | 180 × 180, **no transparency** — cream background baked in | iOS home screen |
| `og-image.jpg` | JPEG | **1200 × 630**, under 300 KB | WhatsApp, Facebook, LinkedIn link previews |

**SVG matters here.** Your mark is fine gold linework and will look soft as a
raster on a retina screen. If only a raster original exists, send the largest
you have and it can be redrawn as SVG.

**`og-image.jpg` is worth doing properly** — it is what people see when the link
is shared on WhatsApp, which is where most of your traffic will come from.
Suggested composition: the hero cow or the signature ghee shot, logo
bottom-left, deep green band, nothing else. It is currently missing entirely,
so shared links show a blank preview.

---

# C. ICONS — 6, already drawn

All six are inline SVG in the page. They inherit the brand colours, scale
perfectly and add zero network requests. **No files needed.** Replace any of
them only if you have a custom icon set.

| Icon | Where it appears | Instances |
|---|---|---|
| Phone handset | Header button, hero CTA, drawer, signature, contact, sticky mobile bar | 6 |
| Long arrow → | Pill CTA buttons | 6 |
| Short arrow → | Product card "Enquire" links | 3 |
| Lab flask | Purity & Quality — "Lab-Tested for Purity" | 1 |
| Shield with tick | Purity & Quality — "FSSAI Compliant" | 1 |
| Concentric circle | Purity & Quality — "Unadulterated" | 1 |

If you commission a custom set: SVG, 24 × 24 viewBox, 1.5 px stroke, no fills,
`stroke="currentColor"` so they pick up the palette automatically.

---

# D. KOLAM AND PATTERN ART — 8 pieces, already drawn

All inline SVG, all using the brand golds and greens. **No files needed.**
Listed so you know what is there and can swap in authentic kolam artwork from a
traditional artist if you want to.

| Piece | Where | What it is |
|---|---|---|
| Brand knot mark | Header, beside the wordmark | Four interlaced loops + four dots, gold — placeholder for your real mark |
| Corner brackets | Hero image, two corners | Kolam line brackets with pulli dots (hidden on mobile) |
| Pulli rail | Left margin of most sections | 1px gold rule with three dots — the site's spine |
| Sikku wave connector | Between the six process steps | Continuous interlaced wave |
| Animated pulli kolam | "A South Indian Morning" | 9 dots, diamond, square, four loops — **draws itself on scroll** |
| Signature watermark | Behind the signature product | Large faint four-petal kolam |
| Philosophy watermark | Behind the brand quote | Large faint sikku kolam on green |
| Footer band | Bottom of the footer | Repeating sikku tile, full width |
| Dot grid | Map placeholder | Pulli grid |

**If you commission real kolam art:** supply as SVG with **strokes, not filled
outlines** — the morning kolam animates by drawing its stroke, which only works
on real paths. Single colour, no background.

---

# E. OPTIONAL — not required

| Asset | Why you might want it |
|---|---|
| Paper or linen texture, seamless PNG ~400 × 400, very low contrast | Adds warmth under the cream ground. Skip unless the brand wants it — it costs page weight for a subtle effect. |
| FSSAI licence mark | Once the licence number is confirmed, it goes in the footer as text; no image needed. |
| Certification marks | Only once certificates actually exist. |

---

# Priority order

If the shoot has to be staged, this is the order that unblocks the most:

1. `hero-cow.webp` — nothing else sets the tone
2. `signature-product.webp` — the ghee itself
3. `product-250ml / 500ml / 1l` — the three jars
4. `logo.svg` + `logo-light.svg`
5. `household-band.webp` — the full-bleed emotional frame
6. The six process steps — one batch, one session
7. The remaining cow and farm frames
8. Food, botanicals, story
9. `og-image.jpg`

---

# What to avoid, in every frame

- Generic Western or European cattle; European-looking farms
- Western-looking people; artificial studio backdrops
- Over-retouched, plastic AI faces
- Food styled for a catalogue rather than cooked
- Heavy filters, crushed blacks, orange-and-teal grading
- Excessive temple or religious imagery
- Bollywood-style lighting and posing

Warm, natural, documentary. If a frame looks like it came from a stock library,
it is wrong for this brand.


---

# Known issues

**1. The hero label shows a price.** `Homepage .png` — now the hero image —
has "₹680" and "1000ml" printed on the jar label. The brief says the site
carries no pricing, and at hero size the figure is legible. Two ways out:
re-render the pack shot without the price, or accept it as printed MRP on the
physical pack. Your call — say the word and I will swap it.

**2. One pack shot serves three sizes.** The 250 ml, 500 ml and 1 L cards all
use the same jar photograph, cropped progressively tighter so the jar reads
larger as the pack gets larger. It looks right, but the cards claim three
sizes and show one. Three real size-specific photographs would fix it
properly — or one frame with all three packs together.

**3. `og:image` uses a relative path.** Social scrapers need an absolute URL.
Once the domain is known, change it to `https://yourdomain.com/assets/og-image.jpg`.

**4. No family photograph.** The Our Story tile marked "family or founder"
currently holds a cow-and-calf frame. A genuine photograph of the people
behind SATVA would do more for trust than anything else on the page.

**Unused source files** (in `~/Documents/Ghee`, deliberately not published):

| File | Why |
|---|---|
| `Morning Churn in a South Indian Home.png` | The placeholder brief is burned into the pixels as caption text. Best composition of the set for the full-width band — worth re-rendering clean. |
| `Rustic Pure Desi Ghee Still Life.png` | The jar is labelled "Pure Desi Ghee", not SATVA. |
| `Elegant Indian Lotus Mandala Backdrop.png` | Orange/red/maroon — off the green-white-gold palette. |
| `Minimal Maroon Kolam Invitation Border.png` | Maroon, off palette; the site's kolam is drawn in SVG. |
| `Golden Morning in a Tamil Village.png` | Replaced as the lead farm tile by `Cow farm.png`. |
| `Sunrise Courtyard with Cow and Calf.png` | Replaced in Our Story by the original hero frame. |
