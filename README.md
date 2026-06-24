# rxVoice2

Landing page for **Formulary** — a once-daily compounded formula, dispensed for a sample size of one.

A single self-contained `index.html` (no build step, no dependencies). The hero pairs a large foreground phone "scanning" a smaller, further-back prescription bottle to sell a sense of depth and perspective. The phone's viewfinder is locked onto the QR code printed on the bottle label via a small positioning script, so the two stay aligned as the window resizes.

## Live page

https://ianpilon.github.io/rxVoice2/

## Highlights

- **Forced-perspective composition** — the phone renders at 2x scale in the foreground while the bottle photo is drawn at half its cover size, so it reads as further away.
- **QR lock** — the bottle photo and the phone share one scale/position source in JS, keeping the phone's scan brackets centered on the bottle's QR code at any width.
- **Balanced layout** — the phone auto-centers in the open space to the right of the copy, with equal whitespace on either side.
- **Clickable scan CTA** — the "Scan QR code" button sits above the fold and re-arms the scan sweep on tap.
- **Responsive** — below 900px the phone is hidden and the bottle reflows for small screens.

## Type & color

- Type: Newsreader (display serif), IBM Plex Sans (body), IBM Plex Mono (labels/metadata).
- Palette: warm studio gray backdrop, near-black ink, amber bottle plastic, mustard label bars, and a maroon hairline accent.

## Running locally

Open `index.html` in any browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```
