<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=42&pause=1000&color=007ACC&center=true&vCenter=true&width=600&height=80&lines=Rootify;Pedigree+Creator;Family+Tree+Builder" alt="Rootify" />

<br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=14&pause=2000&color=4EC9B0&center=true&vCenter=true&width=600&height=30&lines=A+VS+Code-themed+pedigree+chart+builder+%E2%80%94+zero+dependencies" alt="tagline" />

<br/><br/>

![Version](https://img.shields.io/badge/version-2.0-007acc?style=flat-square)
![HTML](https://img.shields.io/badge/HTML-single--file-E34F26?style=flat-square&logo=html5&logoColor=white)
![Canvas](https://img.shields.io/badge/Canvas-HTML5-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/license-MIT-4EC9B0?style=flat-square)
![Theme](https://img.shields.io/badge/theme-VS%20Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![No Dependencies](https://img.shields.io/badge/dependencies-none-569CD6?style=flat-square)

</div>

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=9999&color=DCDCAA&center=true&vCenter=true&width=500&height=50&lines=%E2%9C%A8+What%27s+New+in+v2.0" alt="New in v2" />
</div>

> **12 new features** have been added in v2.0 — listed below in full:

| # | Feature | Shortcut |
|---|---------|----------|
| 🆕 1 | **Undo / Redo** — full 80-step history stack | `Ctrl+Z` / `Ctrl+Y` |
| 🆕 2 | **Double-click to Rename** — floating inline name editor on canvas | `Dbl-click` |
| 🆕 3 | **Snap to Grid** — toggle 40 px snap for clean alignment | Title bar toggle |
| 🆕 4 | **Zoom +/− Buttons** — on-canvas controls in the bottom-right corner | `+` / `−` |
| 🆕 5 | **Miscarriage / Stillbirth Symbol** — small filled triangle per standard notation | `I` key |
| 🆕 6 | **Auto-Arrange Generations** — one-click layout tidying sorted by Y-band | Sidebar button |
| 🆕 7 | **Duplicate Individual** — clone selected with all properties intact | `Ctrl+D` |
| 🆕 8 | **Arrow Key Nudging** — move selected 10 px (1 px with `Shift`) | `↑ ↓ ← →` |
| 🆕 9 | **Generation Guide Lines** — faint horizontal bands behind each generation | Title bar toggle |
| 🆕 10 | **Stats in Status Bar** — live count of affected individuals and carriers | Always visible |
| 🆕 11 | **Birth Year Field** — attach a year rendered as `b.1952` sub-label | Properties panel |
| 🆕 12 | **Notes & Hover Tooltip** — write clinical notes, shown on 600 ms hover | Properties panel |

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=9999&color=569CD6&center=true&vCenter=true&width=500&height=50&lines=%F0%9F%94%AC+Overview" alt="Overview" />
</div>

**Rootify** is a browser-based pedigree chart builder styled after Visual Studio Code. It runs as a **single HTML file** — no server, no build step, no package manager required. Open it in any modern browser and start building clinical-grade family pedigrees immediately.

It implements the full set of standard symbols used in medical genetics pedigrees, combined with a familiar VS Code dark interface that feels natural to anyone who writes code.

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=9999&color=4EC9B0&center=true&vCenter=true&width=500&height=50&lines=%F0%9F%A7%AC+Symbols+%26+Individuals" alt="Symbols" />
</div>

### Standard Pedigree Symbols

| Symbol | Gender | Meaning |
|--------|--------|---------|
| □ Square | Male | Unaffected |
| ■ Filled Square | Male | Affected |
| ◪ Half-filled Square | Male | Carrier |
| ○ Circle | Female | Unaffected |
| ● Filled Circle | Female | Affected |
| ◐ Half-filled Circle | Female | Carrier |
| ◇ Diamond | Unknown | Unaffected |
| ◆ Filled Diamond | Unknown | Affected |
| △ Triangle | Any | Miscarriage / Stillbirth |
| Symbol + slash | Any | Deceased |
| Symbol + teal arrow | Any | Propositus (index case) |

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=9999&color=CE9178&center=true&vCenter=true&width=500&height=50&lines=%F0%9F%94%97+Relationship+Lines" alt="Relationships" />
</div>

Rootify supports all five standard pedigree relationship lines, drawn on HTML5 Canvas with intelligent automatic routing:

**Marriage** connects two individuals with a single horizontal line at their midpoint. **Consanguineous marriage** renders a double horizontal line indicating biological relation. **Descent / Child** links a child to its parents — if the first selected parent is already in a married couple, the descent line automatically routes from the couple's midpoint. **Twins** branch two lines from a shared apex above both siblings. Identical twins add a crossbar connecting the two descent lines.

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=9999&color=DCDCAA&center=true&vCenter=true&width=500&height=50&lines=%F0%9F%8F%B7%EF%B8%8F+Auto+Labelling" alt="Auto Labelling" />
</div>

Individuals are automatically assigned compound labels based on canvas position. Rootify clusters individuals into generations by vertical proximity (±55 px), sorts them left to right by X coordinate, and assigns labels in the form **generation-position** (e.g. `II-3`, `III-7`). Generation Roman numerals are rendered as a floating overlay on the left edge, updating live as individuals move. Double-click any individual to open an inline name editor — the name replaces the auto-label in all rendered output and exports.

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=9999&color=007ACC&center=true&vCenter=true&width=500&height=50&lines=%F0%9F%8E%A8+UI+Design" alt="UI Design" />
</div>

### VS Code Layout

```
┌─ Title Bar (30px) ──────────────────────────────────────────────┐
│ ● ● ●  │  Rootify — pedigree-creator.ped  │ ⊞ Snap │ ⊟ Guides  │
├────────┬────────────────────────┬──────────────────────────────┤
│  Act.  │  Sidebar               │  Canvas Editor               │
│  Bar   │  ├── Tools             │  · · · · · · · · · · · ·    │
│        │  │   ├─ Individuals    │  · · · · · · · · · · · ·    │
│        │  │   ├─ Relationships  │                         [+]  │
│        │  │   └─ History        │                         [⊙]  │
│        │  ├── Properties        │                         [−]  │
│        │  └── Legend            │                              │
├────────┴────────────────────────┴──────────────────────────────┤
│ Status Bar — tool │ count │ affected │ carriers │ zoom │ pos   │
└─────────────────────────────────────────────────────────────────┘
```

### Colour Palette

| CSS Variable | Hex | Usage |
|---|---|---|
| `--bg` | `#1e1e1e` | Canvas background |
| `--bg-panel` | `#252526` | Sidebar, activity bar |
| `--bg-sidebar` | `#2c2c2c` | Tool button fills |
| `--bg-titlebar` | `#323233` | Title bar |
| `--bg-sel` | `#04395e` | Active selection fill |
| `--accent` | `#007acc` | Highlights, status bar, active borders |
| `--text` | `#cccccc` | Primary text |
| `--text-dim` | `#858585` | Labels, hints, dimmed UI |
| `--text-blue` | `#569cd6` | Property values, IDs |
| `--text-teal` | `#4ec9b0` | Propositus arrow, connection highlight |
| `--red` | `#f44747` | Danger / delete actions |
| `--yellow` | `#dcdcaa` | Section headings |

### Typography

**JetBrains Mono** is used throughout — the same typeface shipped with JetBrains IDEs and widely adopted in VS Code via extensions. Its precise monospaced forms give Rootify an unambiguously technical character. Fallbacks: `Consolas → monospace`. The canvas grid uses a 20 px radial-dot pattern to provide spatial reference without visual noise.

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=9999&color=4EC9B0&center=true&vCenter=true&width=500&height=50&lines=%E2%8C%A8%EF%B8%8F+Controls" alt="Controls" />
</div>

### Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `V` / `Esc` | Select tool |
| `M` | Place Male |
| `F` | Place Female |
| `U` | Place Unknown |
| `I` | Place Miscarriage / Stillbirth |
| `R` | Marriage line |
| `K` | Consanguineous line |
| `C` | Child / descent |
| `T` | Twin lines |
| `Ctrl+Z` | Undo |
| `Ctrl+Y` / `Ctrl+Shift+Z` | Redo |
| `Ctrl+D` | Duplicate selected |
| `↑ ↓ ← →` | Nudge selected (10 px) |
| `Shift + ↑ ↓ ← →` | Fine nudge selected (1 px) |
| `Del` / `Backspace` | Delete selected |
| `Ctrl+0` | Reset view (pan & zoom) |
| `Dbl-click` | Inline rename editor |

### Mouse Controls

| Action | Result |
|--------|--------|
| Click empty canvas (place tool) | Place new individual |
| Click individual (select tool) | Select |
| Drag | Move individual |
| Scroll | Zoom in / out |
| `Alt` + drag | Pan canvas |
| Middle-click + drag | Pan canvas |
| Right-click individual | Context menu |
| Double-click individual | Inline rename |
| Hover individual (600 ms) | Notes tooltip |

### Connection Workflow

```
1. Pick Marry / Consang. / Child / Twin tool
2. Click first individual  →  dashed blue preview line appears
3. Click second individual →  relationship is drawn

For Child: if the first parent is already married, the descent
line automatically routes from the couple's midpoint.
```

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=9999&color=569CD6&center=true&vCenter=true&width=500&height=50&lines=%F0%9F%93%8B+Properties+Panel" alt="Properties" />
</div>

Selecting any individual opens the **Properties** panel. Each individual supports:

**Auto ID** — read-only compound label computed from generation position (e.g. `III-2`). **Name** — free-text, rendered below the symbol on canvas and in exports. **Birth Year** — numeric year shown as `b.1952`. **Gender** — Male, Female, Unknown, or Miscarriage. **Affectedness** — Unaffected or Affected. **Modifiers** — Carrier, Deceased, and Propositus can all be active simultaneously. **Notes** — multi-line clinical observations shown in a hover tooltip. **Duplicate** — clones the individual 50 px offset. **Delete** — removes the individual and all connected relationships.

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=9999&color=CE9178&center=true&vCenter=true&width=500&height=50&lines=%E2%AC%87%EF%B8%8F+Export" alt="Export" />
</div>

**Export as PNG** renders the full pedigree to a high-quality image. The engine crops tightly to all individuals, adds 60 px padding, applies a `#1e1e1e` dark background, and includes all labels, symbols, relationship lines, and generation markers. Output is saved as `rootify-pedigree.png`.

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=9999&color=DCDCAA&center=true&vCenter=true&width=500&height=50&lines=%F0%9F%97%82%EF%B8%8F+File+Structure" alt="File Structure" />
</div>

```
rootify.html
├── <style>           CSS variables, layout, VS Code component styles
├── <canvas>          HTML5 Canvas drawing surface
├── #gen-labels       Floating Roman numeral overlays
├── #rename-wrap      Inline rename input
├── #tooltip          Hover notes tooltip
├── #zoom-ctrl        +/⊙/− zoom buttons
├── #ctx              Right-click context menu
├── #statusbar        Tool │ count │ affected │ carriers │ zoom │ pos
└── <script>          ~500 lines vanilla JS — zero dependencies
    ├── State (S)     Single object for all application state
    ├── History       80-step undo/redo stack (JSON snapshots)
    ├── Render        Canvas draw loop — guides, relationships, individuals
    ├── Hit test      Reverse-order point-in-shape test
    ├── Mouse/KB      Drag, pan, zoom, keyboard shortcuts
    ├── Properties    Dynamic property panel generator
    └── Export        Off-screen canvas → PNG download
```

The only network request is the **JetBrains Mono** Google Fonts stylesheet. The app works fully offline, falling back to `Consolas → monospace`.

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=9999&color=28C840&center=true&vCenter=true&width=500&height=50&lines=%F0%9F%8C%90+Browser+Compatibility" alt="Browser Compatibility" />
</div>

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 90+ | ✅ Full support |
| Firefox | 88+ | ✅ Full support |
| Safari | 14+ | ✅ Full support |
| Edge | 90+ | ✅ Full support |

---

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=13&pause=3000&color=858585&center=true&vCenter=true&width=500&height=30&lines=MIT+License+%E2%80%94+free+to+use%2C+modify%2C+and+distribute" alt="license" />

<br/>

**Rootify** — *because every family tree deserves a clean commit history.*

</div>
