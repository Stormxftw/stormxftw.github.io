# Strugglehugs — personal site

A single-file personal website for **Strugglehugs (@Stormxftw)**, built with the
techniques from [teknium.io](https://teknium.io/) and catered to this rig, these
projects, and this persona.

## Open it

Double-click `index.html`. Everything is embedded (images included) — no build
step, no server, no dependencies. Google Fonts load from the network when
online; offline it falls back to local monospace/serif faces and still works.

## What's inside

| Section | Technique (after teknium.io) | Personalization |
|---|---|---|
| Boot gate | BIOS probe lines + PRESS ANY KEY | Real rig specs, 133 skills, 57 worktrees |
| Ticker | Scrolling JP/EN marquee | FL Studio, VoiceMeeter, Neon Rain, the Wired |
| 01 · now | Hero + stat sparklines + terminal replay | Real GitHub/local counts; replay ends with a rule Hermes actually saved to the Pulsr dev skill |
| 02 · rig | Tabbed interactive panel (his is ratatui/WASM; this is canvas) | RIG specs · AGENTS fan-out · SIGNAL audio chain |
| 03 · the mix | Draggable equalizer presets (his dsssp metaphor) | Six real projects as EQ presets — agents/code/audio/visuals/game/web |
| 04 · story | Physics word-field ("drag the world") + timeline | Code Louisville 2016 → Pulsr hackathon Nov 2026, dates from GitHub |
| 05 · shelf | ascii-fx hover on project screenshots | Pulsr, Nest for Raven, ReadLatch (real screenshots) |
| 06 · signals | Writing/link list | Repos, specs, and the old persona site |

Palette: **Neon Rain** — the exact scheme from `herdr-nightcity/windows-terminal/neon-rain.json`.
Mascot: **Volt Ronin**, the cyber-fox gif from the old `personal-website` repo.
Type: JetBrains Mono + Space Grotesk + Instrument Serif italic + VT323 (boot).

Accessibility & behavior: keyboard-operable EQ points (arrow keys) and panel
tabs, `prefers-reduced-motion` honored throughout (instant boot, static ticker,
instant replay, no word physics), mobile layout with a vertical signal chain,
no trackers/cookies. Boot shows once per tab session; the footer **↻ reboot**
replays it.

## Deploy (GitHub Pages)

The `personal-website` repo already has a Pages workflow. Either:

1. Replace its `index.html` with this file (keep or delete the old assets), or
2. Make a new repo (e.g. `strugglehugs.github.io` or `site`), commit
   `index.html`, and enable Pages on the branch root.

`assets/` here holds the optimized source images for future edits — they are
already base64-embedded in `index.html`, so deploying the single file is enough.

## Customize

All content lives in `index.html`:

- `BOOT_LINES`, `TICKS` — boot screen and ticker
- `RLINES` — terminal replay script
- `SPARKS` + the `.stats` markup — counters (refresh from GitHub when needed)
- `PRESETS` / `BANDS` — equalizer projects and band values
- `#wordfield` text + `.timeline` — story and log
- `.cards` / `.also` / `.signals` — shelf and links

## Honesty notes

- Counts are real (GitHub API + this machine, Nov 18 2026); sparkline shapes
  are illustrative and labeled as such on the page.
- The terminal replay is hand-authored and labeled; its last line is a real
  saved skill rule: "unattended proposals never automatically preview."
- RIG load bars and the AGENTS fan-out animation are illustrative; specs,
  worktree count, and the audio chain are real.
- The EQ is a metaphor, not a benchmark — labeled on the page.

Credits: techniques inspired by teknium.io · palette from herdr-nightcity ·
Volt Ronin from the previous persona site · built with Hermes Agent.