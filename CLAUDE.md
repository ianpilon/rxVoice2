# rxVoice2 — project notes for Claude

## Design skill (use this for any design work here)

This project is designed using the **DESIGN.md** design skill / format from
Google Labs: https://github.com/google-labs-code/design.md

When returning to this project for any visual/design change (layout, type,
color, spacing, motion, components), **load and use DESIGN.md again** so the
design language stays consistent across sessions. Do not switch to a different
design skill unless explicitly asked.

- The format: YAML front-matter design tokens (`colors`, `typography`,
  `rounded`, `spacing`, `components`) plus a markdown body whose prose is the
  real source of truth, in the canonical section order (Overview → Colors →
  Typography → Layout → Elevation → Shapes → Components → Do's and Don'ts).
- Philosophy: prose over tokens; a *specific reference* beats a list of
  adjectives; negative constraints (the "don'ts") define the character.
- Tooling: `npx @google/design.md lint|diff|export|spec`.

## The page

`index.html` is the whole site (no build step). Hero is a forced-perspective
composition: a 2x foreground phone whose scan viewfinder is locked onto the QR
code of a half-scale prescription bottle. The bottle photo and the phone share
one scale/position source in the inline `place()` script — keep them coupled.
