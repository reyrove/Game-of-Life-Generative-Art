# Game of Life — Generative Art

> A cellular automaton study for textile and surface design.  
> A reproducible catalogue of computational compositions.

---

## What is this?

**Game of Life** is a generative design system built on Conway's four rules. Cells are born, live, and die according to their eight neighbours — and from that simple rule-set, complex patterns emerge: gliders, oscillators, beehives, endless travelling shapes.

Every artwork in this catalogue is defined by a random seed. Each composition — its grid, palette, and initial density — is generated fresh on every run, making the output **emergent, reproducible, and licensable** across textile, print, and apparel applications.

Where **Arachne** spins concentric rings, **Game of Life** works cell by cell — the same interest in rule-based surface, approached through a different engine.

---

## Live

🌐 **[View the catalogue →](https://reyrove.github.io/Game-of-Life-Generative-Art/)**

---

## The System

The generator combines two layers:

| Layer | Description |
|-------|-------------|
| **Grid** | A 100×100 to 300×300 cell matrix, seeded at ~6% density. |
| **Evolution** | Conway's four rules applied per generation — birth, survival, death. |

Both are driven by a random seed at load, ensuring every refresh produces a distinct composition.

### Parameters

- **Grid size** — 100 to 300 cells per row/column
- **Background colours** — 28 dark, saturated options
- **Foreground colours** — 28 bright, high-contrast options
- **Initial density** — ~6% random live cells
- **Simulation speed** — 10 frames per second

---

## Structure

```
Game-of-Life-Generative-Art/
├── index.html          ← Full catalogue (single-file)
├── images/
│   └── fav.svg
├── Game-of-Life.jpg    ← Apparel mockup
├── README.md
└── LICENSE
```

The entire project is contained in a single `index.html` — no build step, no dependencies beyond p5.js loaded from a CDN. Open it in any modern browser.

---

## Features

- **Seed-based generation** — every composition is emergent and documented
- **Live catalogue** — cover, plate, surfaces, process, archive, commission sections
- **Multiple surfaces** — print, scarf, textile, wallpaper — all rendered from the same generation
- **Archive of 8 plates** — click any plate to load it into the main view
- **PNG export** — download any composition directly from the browser
- **Keyboard shortcuts** — `R` for new seed, `S` to download
- **Legal modal** — licensing, terms, and credits built in
- **Responsive** — works on desktop, tablet, and mobile
- **Mobile-first navbar** — horizontally scrollable with fade hint

---

## Usage

### Generate a new composition

Click **New Seed** or press `R`.

### Download the current composition

Click **Download** or press `S`.

### Load a seed from the archive

Click any plate in the **Archive** section.

---

## Color System

Each composition is assigned a palette drawn from two independent pools:

- **Background** — 28 dark tones, from pure black to deep aubergine
- **Foreground** — 28 bright tones, from bone white to electric cyan

Each run selects one background and one foreground at random — producing high-contrast pairings that let the cellular structure read clearly at any grid size.

---

## The Game of Life Rules

Conway's Game of Life follows four simple rules:

1. **Underpopulation** — Any live cell with fewer than 2 live neighbours dies
2. **Survival** — Any live cell with 2 or 3 live neighbours lives on
3. **Overpopulation** — Any live cell with more than 3 live neighbours dies
4. **Reproduction** — Any dead cell with exactly 3 live neighbours becomes alive

Despite these simple rules, complex and beautiful patterns emerge.

---

## Technical Notes

- Pure vanilla JavaScript with p5.js for the sketch
- Canvas 2D rendering
- Custom matrix of `Uint8Array` rows for fast neighbour counting
- Integer-aligned cell drawing for crisp output at any grid size
- Device-pixel-ratio aware rendering
- Toroidal simulation — edges wrap instead of dying

---

## About

**Game of Life** is a project by [Reyhaneh Daneshdoost](https://reyrove.github.io/) — an Iranian-born artist working at the intersection of classical textile logic and generative systems.

The work begins with a simple observation: the woven surface — repetitive, mathematically structured, infinitely variable — has always been a form of computation, long before computers.

**Game of Life** is a companion volume to Arachne, treating Conway's rule-set as a textile system.

> *Four rules. No designer. Yet the grid keeps producing form.*

---

## Licensing

All compositions are documented and available for licensing across textile, surface, and apparel applications.

For commercial use, custom editions, or exclusive rights:

📧 **reyhanehdaneshdoost@gmail.com**

See the **Licensing** section in the live catalogue for details.

---

## Links

- 🌐 [Website](https://reyrove.github.io/)
- 📷 [Instagram](https://www.instagram.com/rey._.rove/)
- 💼 [LinkedIn](https://www.linkedin.com/in/reyhaneh-daneshdoost-730481160/)
- 🐦 [X](https://x.com/reyrove)

---

## Credits

**Design & Generative System**  
Reyhaneh Daneshdoost

**Typefaces**  
Cormorant Garamond · DM Mono

**Automaton**  
Conway's Game of Life (1970)

**Edition**  
Game of Life — Autumn 2026

---

<p align="center">
  <em>Cellular Automaton · Textile Design</em><br />
  <sub>© Reyrove Studio · All compositions reproducible by seed</sub>
</p>