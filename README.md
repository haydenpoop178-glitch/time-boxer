# Time Boxer

A visual day planner. Drag on a timeline to block out chunks of time, label them,
and let a live countdown keep you honest about the current block.

## Run it

Just open `index.html` in a browser — no build, no server, no dependencies.

```bash
open index.html
```

## How it works

- **Day grid** — 6:00 AM to midnight in 15-minute slots.
- **Drag to create** — click-drag vertically on the grid to paint a block. The
  label editor pops open automatically. Blocks can't overlap.
- **Click a block** — rename it, recolor it, or delete it.
- **Now card** (top) — shows the block you're in, a ring that fills as it elapses,
  and minutes remaining. Between blocks it shows how long you're free and what's
  coming up next.
- **Red now-line** — tracks the current time across the grid.
- **Chime** — a soft three-note tone plays when a block ends. Toggle with the
  bell button (also unlocks browser audio on first click).
- **Persistence** — everything is saved to `localStorage` in that browser, so a
  refresh keeps your plan. "Clear day" wipes it.
- **Add to Calendar** — downloads a `.ics` file of today's blocks. Double-click it
  and Apple Calendar (or Google Calendar) will ask which calendar to add the
  events to. One-way snapshot: it does not sync back, and re-exporting creates a
  fresh set of events rather than updating the old ones.

## Everything is in one file

`index.html` — markup, styles, and ~350 lines of vanilla JS. No frameworks.
Theme follows your OS light/dark setting.
