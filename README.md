# SATVA Pure Cow Ghee — website

One static page. No build step, no dependencies, no server logic, no database.
`index.html` is the whole site; `assets/` holds the photographs.

```
index.html      the site (73 KB, all CSS and JS inline)
assets/         27 photographs as WebP + og-image.jpg  (3.0 MB)
README.md       this file
ASSETS.md       full asset manifest and open items
```

## Putting it online

Upload the **contents** of this folder — `index.html` and the `assets/` folder
side by side — to any static host. Nothing needs installing or configuring.

Netlify or Cloudflare Pages: drag the folder onto the dashboard.
cPanel or FTP hosting: drop it in `public_html/`.
GitHub Pages: push the folder and enable Pages on the branch.

To preview locally:

```bash
python3 -m http.server 8777
```

Then open `http://localhost:8777/`. Opening `index.html` straight from Finder
works too, though some browsers restrict local file loading.

## Before you go live

- Replace the placeholder logo mark with the real `logo.svg` (section 1)
- Set `og:image` to an absolute URL once the domain is known (see ASSETS.md)
- Add the FSSAI licence number to the footer
- Add the Google Maps embed and `LocalBusiness` schema once the address is set

## 1. The logo

In the header, find:

```html
<img id="brand-logo" src="" alt="" hidden>
<span class="wordmark"><b>SATVA</b><span>Pure Cow Ghee</span></span>
```

Set `src="assets/logo.svg"` (SVG preferred, transparent PNG at 2× also fine).
The typographic wordmark removes itself automatically once a real logo is set.

Until then the header shows a **placeholder gold knot mark** drawn in SVG, in
the spirit of the supplied logo lockup. It is not a copy of your mark — send
the real file and it is one line to swap.
The footer carries its own copy of the wordmark — swap that one by hand.

## 2. Brand colours — supplied SATVA palette

Every colour on the page comes from nine tokens at the top of the `<style>` block,
weighted to the 60 / 20 / 10 / 5 / 5 hierarchy in the brand guide:

```css
--cream:#F7F1E3;      /* 60% — main background                   */
--off-white:#FFFDF7;  /*       cards, product sections           */
--forest:#314A35;     /* 20% — brand / heritage bands, headings  */
--gold:#D6A83A;       /* 10% — ghee gold, kolam dots, highlights */
--terracotta:#A85A3A; /*  5% — kolam linework, labels, hovers    */
--brown:#3A2A20;      /*  5% — typography                        */
--olive:#68704A;      /*       secondary accent (farm section)   */
--brass:#B78A3A;      /*       premium details, hairlines        */
--sand:#EDE3CC;       /*       image placeholder panels          */
```

Two notes on how the palette is used:

- **Ghee Gold and Brass Gold are never set as small text.** At `#D6A83A` and
  `#B78A3A` they land near 3:1 on cream, which fails legibility for the small
  uppercase eyebrows and numerals. Those use Terracotta instead, and the golds
  carry every kolam line, dot, hairline and the footer band — which is where
  they look best anyway.
- **Forest appears twice as a full band** (Purity & Quality, and Brand
  Philosophy) plus the footer. That is roughly the 20% the guide asks for
  without tinting the whole page green.

## 3. Typography — per the brand guide

Both faces load from Google Fonts in the page head.

| Role | Face | Size / line-height | Weight |
|---|---|---|---|
| H1 hero | Cormorant Garamond | 60 / 72 px | Semibold |
| H2 section | Cormorant Garamond | 40 / 52 px | Semibold |
| H3 sub-heading | Manrope | 20 / 30 px | Medium |
| Body | Manrope | 16 / 26 px | Regular |
| Navigation | Manrope | 16 px | Medium |
| Button text | Manrope | 16 px | Semibold |
| Small labels | Manrope | 14 px | Medium |

Headings use `clamp()` so they scale down on phones and land exactly on the
guide's sizes from tablet width up — a fixed 60px hero would overflow a 375px
screen. Product names stay in Cormorant Garamond, as the guide specifies.

One documented exception: the **header** Call Us button uses the 14px label
size rather than 16px. At 16px semibold uppercase it crowded the navigation on
laptop widths. Every other button on the page is 16px semibold.

## 4. Photographs

Every photograph is a real `<img>` inside a `.slot` wrapper, cropped to fill by
`object-fit: cover`. To swap one, replace the file in `assets/` keeping the same
name, or point the `src` at a new file — and update its `alt` text, which is
what screen readers and search engines read.

All images except the hero are lazy-loaded. The hero is `fetchpriority="high"`
so it paints first.

**The full shot list, logo files, icon and pattern inventory live in
[ASSETS.md](ASSETS.md)** — 27 photographs with ratios, pixel sizes, formats and
filenames, plus what is already drawn in SVG and needs no file at all.

Shot list in page order — the on-page placeholder label is the brief:

| Section | Shot |
|---|---|
| Hero | Native cow on a Tamil Nadu farm, tiled-roof house, coconut and banana trees, brass milk vessel, morning light |
| The SATVA Story | Traditional South Indian kitchen, brass vessels, window light |
| Our Ghee | Three product photographs — 250 ml, 500 ml, 1 L |
| Signature | Hero product shot — jar, brass spoon, golden ghee |
| The Household | Full-width documentary frame — woman in saree at a wooden churner |
| Where Tradition Begins | Five farm frames — grazing cow, cow and calf, farmer, milking, landscape |
| One Spoon | Three food frames — ghee over ven pongal, paruppu sadam, payasam |
| A South Indian Morning | Kolam at the doorstep, tulasi maadam, sunrise |
| From Milk to Golden Ghee | Six square process frames — milk, curd, churning, butter, heating, ghee |
| Our Story | Family, farm, product in a traditional setting |

Suggested sizes: full-width bands 2400px wide, editorial slots 1600px,
product cards 1200px. JPEG at ~80% quality; keep each file under ~350 KB.

## 5. Google Maps

**Removed for now.** The map panel and the "Get Directions" button are gone —
they were placeholders pointing nowhere, and a dead button costs more trust than
a missing one. The Contact section now runs Call / Email / Timings as three
columns with Call and Email as the actions.

When the address is confirmed, the map comes back as a Google Maps `<iframe>`
in the Contact section, plus a `LocalBusiness` schema block.

## 6. Copy, and what is still open

The About Us text supplied by the brand is now live across the site:

| Brand copy | Where it sits |
|---|---|
| Our Philosophy | The SATVA Story section, and *Our Story → What we believe* |
| The Traditional Process | *From Milk to Golden Ghee* — the six-step timeline and the note beneath it |
| Our Signature Infusion | Its own section, with moringa and cumin as named botanicals |
| Uncompromising Purity & Quality | The forest-green *Trust Is Earned Through Transparency* band |
| Our Offerings | Product cards and the signature product section |

Still open:

- **FSSAI licence number.** The site states FSSAI compliance in words. Indian
  packaged-food sites normally display the licence number itself — send it and
  it goes in the footer, where buyers look for it.
- **Lab test reports.** "Lab-tested for purity" is stated. If you can share a
  report or the testing lab's name, that claim gets much stronger and can have
  its own panel.
- **Health-claim wording.** The supplied copy describes the infused ghee as a
  "nutrient-dense superfood" that "supports daily vitality", and the process as
  retaining "maximum nutritional value". Those are nutrition and health claims
  under FSSAI's advertising rules, which require substantiation. The website
  copy has been kept to what the infusion *is* and how it tastes; the stronger
  wording is held back until you confirm you hold the substantiation. Say the
  word and it goes in verbatim.
- **Cattle breeds.** Still not named anywhere. Add only on confirmation.

## 7. SEO and structured data

`<title>`, meta description and Open Graph tags are set. JSON-LD covers
Organization (phones, email, 8 AM – 9 PM hours) and Product (three sizes, no
prices or offers, because this is not a shop).

Product schema now names the traditional churning, the moringa and cumin
infusion, lab testing and FSSAI compliance — all supplied by the brand. Still
no prices and no offers, because this is not a shop.

A `LocalBusiness` block is intentionally absent — there is a comment marking
where it goes once the street address is supplied. Adding one without a real
address would be false structured data.

## 8. What the site deliberately does not do

No cart, no checkout, no payment, no prices, no ordering, no delivery or
minimum-order information. Every product action is a phone call:
`9791180469` / `9500046659`, plus a sticky click-to-call bar on mobile.
