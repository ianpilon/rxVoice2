# rxVoice2 — Plainscript

Landing page for **Plainscript** — a patient-centred delivery layer for prescription medication information.

Today the information a patient needs to take a medicine safely is fragmented across three documents (a clinician-facing product monograph, a plain-language Patient Medication Information sheet, and the physical bottle label), and at each handoff legibility, comprehensibility, or actionability breaks down. Plainscript turns the label on your bottle into medication information you can actually use: scan it, and the same regulator-approved guidance pharmacists work from becomes large type, plain language, searchable, read-aloud, and translatable.

A single self-contained `index.html` (no build step, no dependencies).

## Live page

https://ianpilon.github.io/rxVoice2/

## The page

- **Hero** — a forced-perspective composition: a large foreground phone "scanning" the QR code on a smaller, further-back prescription bottle. The phone's viewfinder is locked onto the bottle's QR via a small positioning script, so the two stay aligned as the window resizes.
- **The problem** — the three documents (label, leaflet, monograph) and how each fails the patient.
- **How it works** — scan the bottle, read it your way (text size, contrast, plain language, translate), then ask a question or have it read aloud.
- **What you can ask** — the real questions a label never answers ("can I take this with food?", "what do I do if I miss a dose?").
- **One source of truth** — drawn from Health Canada's structured PMI and the machine-readable product monograph; the same authoritative content pharmacists dispense from. No new regulation, no bigger labels.

## Design

Designed with the **DESIGN.md** skill (see `CLAUDE.md`). Apothecary/pharmacy register: Newsreader (display serif), IBM Plex Sans (body), IBM Plex Mono (labels), on a warm studio-gray ground with amber, mustard, and maroon accents.

## Running locally

Open `index.html` in any browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```
