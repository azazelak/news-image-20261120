# World News — Friday 20 November 2026, in one image

make.fun entry for `news-image-20261120`: "Sum up 20 November's world
news in one image". A Node 22 program (`main.ts`, standard library
only, no network) draws a 1024×1024 PNG of the day's news and writes
it to `$MAKEFUN_OUTPUT_DIR/entry.png` (default `/output`).

## The image

- **Masthead:** WORLD NEWS — FRIDAY 20 NOVEMBER 2026.
- **Lead story:** Russia's overnight ballistic strikes on three of
  Kyiv's bridges over the Dnipro — three killed, 15 hurt, the
  biggest attack on the capital's crossings since the war began,
  in retaliation for Ukraine's strikes on the Crimean Bridge.
- **11 further stories** in a clean 3×4 grid (not a dense 3×6):
  Europe dismisses the Shenzhen "peace declaration"; COP31's
  endgame with fossil fuels dropped from the draft; Cyclone Akvan's
  landfall in Odisha; the UK–EU youth mobility deal; a Houthi
  missile hitting Riyadh's PIF Tower; Anthropic's Nasdaq debut;
  unknown objects falling near Poland's border; tankers hitting
  mines off Hormuz; Rohingya welcoming the ICJ verdict; Nigeria
  moving to end jail terms for attempted suicide; a M5.6 quake off
  New Caledonia. Footer ticker: Genoa airport halted by drones,
  Japan core inflation at 2.2%.
- Every story was verified against reporting dated 20 November
  2026 — see `BUILD_LOG.md` for the outlet and date of each one.
  Items whose event fell on Thursday evening but were first widely
  reported on Friday are worded as the Friday reporting of them.

## Run

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

Two runs write byte-identical PNGs (no clock, no randomness).
Output is 1024×1024, well under 1 MiB. The program throws if any
headline wraps past 2 lines or any summary past 1 line, so text
can never be silently clipped.
