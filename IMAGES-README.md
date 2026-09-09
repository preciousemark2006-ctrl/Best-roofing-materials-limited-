
The HTML and CSS are already 100% self-contained — no Google Fonts, no external
scripts, nothing loaded from Claude. The only outside dependency left is the
photography, which the page expects to find in an `images/` folder sitting
right next to `index.html`:

```
your-folder/
├── index.html
└── images/
    ├── 01-hero-house-dusk.jpg
    ├── 02-house-under-construction.jpg
    ├── 03-aluminum-sheet-texture.jpg
    ├── 04-stone-coated-tile-texture.jpg
    ├── 05-row-of-modern-houses.jpg
    ├── 06-gallery-red-roof-building.jpg
    ├── 07-gallery-installers-team.jpg
    ├── 08-gallery-sheet-detail.jpg
    ├── 09-gallery-wooden-work.jpg
    ├── 10-gallery-fixing-finishing.jpg
    ├── 11-gallery-architectural-roofline.jpg
    ├── 12-gallery-onsite-installation.jpg
    └── 13-final-cta-house-dusk.jpg
```

## Option A — use your own project photography (recommended)

Best Roofing Materials Limited's real photos will make this site far more
convincing than any stock photo. Shoot or gather photos for each slot above
(a finished roof, a materials close-up, your team on site, etc.), save them
with the exact filenames listed, and drop them in the `images/` folder. No
code changes needed.

## Option B — use the placeholder stock photography this draft was built with

Download each image below (free to use, no attribution required — Unsplash
License) and save it with the matching filename into `images/`:

| Filename | Source page |
|---|---|
| 01-hero-house-dusk.jpg | https://unsplash.com/photos/modern-luxury-house-with-stone-accents-at-sunset-7qD-iDyrdHY |
| 02-house-under-construction.jpg | https://unsplash.com/photos/a-new-house-under-construction-with-a-dark-roof-lT2Hpiqgn3c |
| 03-aluminum-sheet-texture.jpg | https://unsplash.com/photos/dark-grey-roof-tiles-pattern-m_vEaZizd2s |
| 04-stone-coated-tile-texture.jpg | https://unsplash.com/photos/brown-roof-tiles-in-close-up-photography-oPPoyFHG11Q |
| 05-row-of-modern-houses.jpg | https://unsplash.com/photos/row-of-modern-houses-with-interesting-roof-design-sIsiRYz3VKk |
| 06-gallery-red-roof-building.jpg | https://unsplash.com/photos/red-and-black-building-under-blue-sky-wmhhsI7GUQ8 |
| 07-gallery-installers-team.jpg | https://unsplash.com/photos/a-couple-of-people-that-are-on-a-roof-MyBBMM317A4 |
| 08-gallery-sheet-detail.jpg | https://unsplash.com/photos/a-close-up-of-a-roof-with-a-black-shinnel-BqhKviHBODM |
| 09-gallery-wooden-work.jpg | https://unsplash.com/photos/a-person-using-a-drill-to-drill-a-piece-of-wood-dDluNWaVQWA |
| 10-gallery-fixing-finishing.jpg | https://unsplash.com/photos/a-man-in-a-yellow-shirt-is-working-on-a-roof-eFOkg4ZMiBs |
| 11-gallery-architectural-roofline.jpg | https://unsplash.com/photos/black-and-white-glass-building-Mu9uo42SXEY |
| 12-gallery-onsite-installation.jpg | https://unsplash.com/photos/a-man-on-a-roof-working-on-a-roof-G2J41LRaKkE |
| 13-final-cta-house-dusk.jpg | https://unsplash.com/photos/modern-luxury-home-with-large-windows-at-dusk-G48h926L2qo |

On each page, click "Download free" to get the full-resolution JPG, then
rename it to match the filename in the table.

## Fonts

The page now uses system font stacks (Georgia-based serif for headings,
system sans-serif for body text) instead of Google Fonts, so there's no
font-related network request either. If you'd like the exact Fraunces /
Inter look back, you'd need to self-host the `.woff2` files in a `fonts/`
folder and add `@font-face` rules — happy to wire that up if you get me the
font files.

Once the `images/` folder is filled in, `index.html` will run completely
offline — open it straight from disk, no internet connection required.
