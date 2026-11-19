# Strugglehugs — personal site

A single-file personal website for **Strugglehugs (@Stormxftw)**, built with the
techniques from [teknium.io](https://teknium.io/) and catered to this rig, these
projects, and this persona.

**Live: https://stormxftw.github.io/** — served by GitHub Pages from the public
repo [`Stormxftw/stormxftw.github.io`](https://github.com/Stormxftw/stormxftw.github.io)
(branch `main`, root). To update: edit `index.html`, commit, push — Pages
rebuilds in about a minute.

## Open it locally

Double-click `index.html`. Everything is embedded (images included) — no build
step, no server, no dependencies. Google Fonts load from the network when
online; offline it falls back to local monospace/serif faces and still works.

## What's inside

| Section | Technique (after teknium.io) | Personalization |
|---|---|---|
| Boot gate | BIOS probe lines + PRESS ANY KEY | Real rig specs, 133 skills, 57 worktrees |
| Background | WebGL fluid ink (his webgl-fluid), mouse-reactive, dithered | Hand-written stable-fluids sim in the Neon Rain palette |
| Ticker | Scrolling JP/EN marquee | FL Studio, VoiceMeeter, Neon Rain, the Wired |
| 01 · now | Hero + stat sparklines + terminal replay | Real GitHub/local counts; replay ends with a rule Hermes actually saved to the Pulsr dev skill |
| 02 · rig | Tabbed interactive panel (his is ratatui/WASM; this is canvas) | RIG specs · AGENTS fan-out · SIGNAL audio chain |
| 03 · the mix | Draggable equalizer presets (his dsssp metaphor) | Six real projects as EQ presets — agents/code/audio/visuals/game/web |
| 04 · story | Physics word-field ("drag the world") + timeline | Code Louisville 2016 → Pulsr hackathon Nov 2026, dates from GitHub |
| 05 · shelf | ascii-fx hover on project screenshots | Pulsr, Nest for Raven, ReadLatch (real screenshots) |
| 06 · signals | Writing/link list | Repos, specs, and the old persona site |

Palette: **Neon Rain** — the exact scheme from `herdr-nightcity/windows-terminal/neon-rain.json`.
Avatar: a hand-drawn 24×24 SVG pixel mask — hooded chrome, cracked mirror face, one cyan eye slit — that glitches every few seconds and on hover. It replaced Volt Ronin (the old site's fox) on purpose: an identity that keeps recalibrating.
Type: JetBrains Mono + Space Grotesk + Instrument Serif italic + VT323 (boot).

Accessibility & behavior: keyboard-operable EQ points (arrow keys) and panel
tabs, `prefers-reduced-motion` honored throughout (instant boot, static ticker,
instant replay, no word physics), mobile layout with a vertical signal chain,
no trackers/cookies. Boot shows once per tab session; the footer **↻ reboot**
replays it.

## Private repos

Most project repos (ReadLatch, ForKeeps, frontier-relay, agent-wiki,
practical-hermes-skills, sinker, squad, Patchwright, personal-website, …) are
**private**, so the site shows them greyed-out and unlinked — names,
descriptions and screenshots stay, hrefs are removed. Public repos (Pulsr,
nest-for-raven, herdr-nightcity, H.Realms, SlopLens, aura-kit) keep their
links. If you make a repo public later, re-add its `href` in `index.html`
(shelf cards, `.also` chips, timeline, signals rows).

The old `personal-website` repo is private and stays that way; it holds the
previous Codex-card site (now `legacy.html` there) plus a copy of this site.
Its daily `refresh-codex-card` workflow is untouched. GitHub Pages on a private
repo needs a paid plan — that's why this site lives in its own public repo.

## Customize

All content lives in `index.html`:

- `BOOT_LINES`, `TICKS` — boot screen and ticker
- `RLINES` — terminal replay script
- `SPARKS` + the `.stats` markup — counters (refresh from GitHub when needed)
- `PRESETS` / `BANDS` — equalizer projects and band values
- `#wordfield` text + `.timeline` — story and log
- `.cards` / `.also` / `.signals` — shelf and links

`assets/` holds the optimized source images for future edits — they are
already base64-embedded in `index.html`, so deploying the single file is enough.

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