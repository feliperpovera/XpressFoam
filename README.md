# Xpress Foam — Modern Site

Mobile-first rebuild of [xpressfoam.com](https://xpressfoam.com) for Xpress Foam & Supplies, LLC (Hialeah, FL).

**Live:** https://feliperpovera.github.io/XpressFoam/

## What changed vs. the original

- **Hero cut to the bone.** Two words per line ("Any foam. / Any size."), one supporting line, two buttons. The original stacked four paragraphs above the fold.
- **CTA first.** Sticky call button in the header, a permanent two-button action bar at the bottom on mobile (Call / Free quote), and a CTA inside every industry card.
- **Speed.** Single HTML file, zero frameworks, zero web fonts, system font stack, images recompressed (~1 MB total), map iframe loads only on tap.
- **Mobile-first.** Every layout starts at 375px; touch targets are 46–52px; industry cards, gallery and testimonials are swipeable rails that become grids on desktop.
- **Clean UI.** Brand palette sampled straight from xpressfoam.com: black `#000000`, cyan `#45C7E8`, blue `#4092D6`, yellow CTA `#FFFF00`. One type scale, inline SVG icons (no emoji anywhere), 16px inputs (no iOS zoom), automatic dark mode, `prefers-reduced-motion` respected.
- **SEO/local.** LocalBusiness JSON-LD, real meta description, OG tags.

## Structure

```
index.html      # entire site (inline CSS + JS)
assets/         # client photos, optimized
```

## Run locally

```bash
python3 -m http.server 8777
```

## To do before going live

- Point the quote form at a real endpoint (currently opens a prefilled `mailto:`).
- Confirm the receiving email address (`info@xpressfoam.com` is a placeholder).
- Swap in the real logo file (currently a crop of the provided brand image).
