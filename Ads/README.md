# Catfish ad creatives

Drop the banner artwork in this folder using these exact filenames. The site
picks them up automatically — no code change needed. If a file is missing or
fails to load, the slot falls back to the built-in Tamasha Pro house ad.

| File                       | Size required | IAB name    |
| -------------------------- | ------------- | ----------- |
| `leaderboard-728x90.png`   | 728 x 90 px   | Leaderboard |
| `billboard-970x90.png`     | 970 x 90 px   | Billboard   |

The two sizes alternate on every page refresh.

## Important: artwork must be the exact aspect ratio

These slots are very wide and short — 8.1:1 and 10.8:1. Artwork made for any
other shape (a Facebook cover at ~2.6:1, a square post, a poster) cannot fill
them without being cropped to a narrow horizontal band, which cuts off most of
the design. Ask the designer for the two sizes above specifically.

`.jpg` and `.webp` work too — just change the extension in the `AD_SLOTS` array
in `index.html`.

## Click-through

Each slot in `AD_SLOTS` also takes an `href`. Set it to the advertiser's landing
page and the banner opens it in a new tab. Left empty, the banner opens the
Tamasha plans portal instead.
