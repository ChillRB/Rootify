<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=48&pause=1200&color=007ACC&center=true&vCenter=true&width=700&height=90&lines=Rootify;Pedigree+%2B+Genetics+Lab;Family+Tree+Builder" alt="Rootify" />

<br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=14&pause=2500&color=4EC9B0&center=true&vCenter=true&width=700&height=32&lines=VS+Code-themed+pedigree+builder+%2B+Punnett+Square+lab+%E2%80%94+zero+dependencies" alt="tagline" />

<br/><br/>

![Version](https://img.shields.io/badge/version-3.0-007acc?style=flat-square)
![HTML](https://img.shields.io/badge/HTML-single--file-E34F26?style=flat-square&logo=html5&logoColor=white)
![Canvas](https://img.shields.io/badge/Canvas-HTML5-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/license-MIT-4EC9B0?style=flat-square)
![Theme](https://img.shields.io/badge/theme-VS%20Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![No Dependencies](https://img.shields.io/badge/dependencies-none-569CD6?style=flat-square)
![Punnett](https://img.shields.io/badge/Punnett%20Square-built--in-DCDCAA?style=flat-square)

</div>

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=26&pause=9999&color=DCDCAA&center=true&vCenter=true&width=700&height=55&lines=%E2%9C%A8+What%27s+New+in+v3.0" alt="New in v3" />
</div>

> **15 new pedigree features** plus a full **Punnett Square mode** with 4 cross types, 3 dominance models, and live probability output.

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&pause=9999&color=569CD6&center=true&vCenter=true&width=600&height=40&lines=%F0%9F%A7%AC+15+New+Pedigree+Features" alt="15 new features" />
</div>

| # | Feature | How to use |
|---|---------|-----------|
| 🆕 1 | **Save / Load JSON** — full lossless round-trip export and import | `Ctrl+S` / Load button |
| 🆕 2 | **Multi-select** — `Shift+click` to add to selection, move all together | `Shift+click` |
| 🆕 3 | **Drag-box Selection** — rubber-band draw on empty canvas to capture a group | Click-drag empty canvas |
| 🆕 4 | **Zoom to Fit All** — auto-fits viewport to every individual on canvas | `Ctrl+Shift+0` / ⊙ button |
| 🆕 5 | **Zoom to Selection** — fit viewport to selected individuals only | `Ctrl+F` / ⊡ button |
| 🆕 6 | **Search & Highlight** — type a name to glow-highlight matching individuals | Sidebar search bar |
| 🆕 7 | **Light / Dark Theme** — full CSS-variable theme switch, persists in session | `◑ Theme` title bar toggle |
| 🆕 8 | **Trait Color Picker** — assign a custom fill color per individual for affected state | Properties panel |
| 🆕 9 | **Statistics Panel** — live counts for affected %, carriers, gender split, per-generation counts | Actbar chart icon |
| 🆕 10 | **Relationship Deletion** — click a marriage/relationship line to select it, `Del` to remove | Click line → `Del` or right-click → Delete Relationships |
| 🆕 11 | **Space + Drag Pan** — hold `Space` to enter grab mode and drag the canvas (Figma-style) | `Space` + drag |
| 🆕 12 | **Age Auto-Calculation** — birth year field auto-computes and displays current age inline | Properties → Birth Year |
| 🆕 13 | **Notes Dot Indicator** — a small teal dot appears on any individual that has clinical notes | Auto-rendered on canvas |
| 🆕 14 | **Select All** — selects every individual on the canvas in one keystroke | `Ctrl+A` |
| 🆕 15 | **Per-Generation Count** — Roman numeral labels now show member count e.g. `III (4)` | Always visible |

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=22&pause=9999&color=4EC9B0&center=true&vCenter=true&width=700&height=50&lines=%F0%9F%94%AC+Punnett+Square+Mode" alt="Punnett Square" />
</div>

Rootify v3 ships a fully featured genetics calculator accessible via the **Punnett Square** tab in the title bar. It runs entirely client-side with zero dependencies.

### Cross Types

| Mode | Description | Grid |
|------|-------------|------|
| **Monohybrid** | Single-gene cross with two alleles per parent | 2 × 2 |
| **Dihybrid** | Two-gene cross — gametes generated automatically | 4 × 4 |
| **X-Linked** | Sex-linked inheritance with X^A / X^a notation | 2 × 2 |
| **ABO Blood Type** | Full ABO genotype cross (AA, Ao, BB, Bo, AB, OO) | 2 × 2 |

### Dominance Models

| Model | Phenotype Logic |
|-------|----------------|
| **Complete Dominance** | Any uppercase allele → dominant phenotype; both lowercase → recessive |
| **Incomplete Dominance** | Homozygous dominant ≠ heterozygous ≠ homozygous recessive (blended intermediate) |
| **Codominance** | Both alleles expressed simultaneously in heterozygotes |

### Punnett Features

**Allele input** — type any two uppercase/lowercase letter pair (e.g. `Aa`, `TT`, `bb`). Dihybrid accepts four-letter strings (`AaBb`). **Gamete generation** is automatic — dihybrid gametes are computed combinatorially from the input genotype.

**Color-coded grid** — cells are shaded by phenotype class: blue for dominant, red/pink for recessive, teal for heterozygous, amber for intermediate/codominant, and purple for codominant AB pairs.

**Genotype ratios** — every unique genotype with its frequency fraction and percentage. **Phenotype ratios** — grouped by phenotypic outcome under the selected dominance model.

**X-linked presets** — six maternal/paternal combinations covering homozygous dominant, carrier, homozygous recessive females and normal/affected males, with offspring labeled as carrier females, affected females, normal males, and affected males.

**ABO blood type** — accepts the six standard ABO genotypes and maps every offspring combination to a blood type phenotype (A, B, AB, O) with percentage frequencies.

**Custom trait and allele names** — rename the trait, the dominant phenotype, and the recessive phenotype directly in the settings panel. Labels update live in the ratio cards.

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&pause=9999&color=DCDCAA&center=true&vCenter=true&width=600&height=40&lines=%F0%9F%93%8B+All+Pedigree+Features+(v1+%E2%80%94+v3)" alt="All pedigree features" />
</div>

### Individuals & Symbols

All standard pedigree notation is fully supported. Symbols are drawn on an HTML5 Canvas and scale cleanly at any zoom level.

| Symbol | Meaning |
|--------|---------|
| □ Square | Male |
| ○ Circle | Female |
| ◇ Diamond | Unknown gender |
| △ Triangle | Miscarriage / Stillbirth |
| Filled symbol | Affected |
| Half-filled symbol | Carrier |
| Symbol + diagonal slash | Deceased |
| Symbol + teal arrow | Propositus (index case) |
| Custom fill color | User-defined trait color (v3) |
| Small teal dot | Notes attached (v3) |

### Relationship Lines

| Line Type | Meaning |
|-----------|---------|
| Single horizontal | Marriage |
| Double horizontal | Consanguineous (related partners) |
| Vertical drop + horizontal + vertical | Child / descent (auto-routes from couple midpoint) |
| Branching apex lines | Fraternal twins |
| Branching + crossbar | Identical twins |

### Properties per Individual

Every individual on the canvas has the following editable fields: **Auto ID** (read-only, compound Roman/numeric label), **Name** (custom free-text, shown on canvas), **Birth Year** (auto-calculates and displays current age), **Gender** (four-way toggle), **Affected/Unaffected**, **Carrier** modifier, **Deceased** modifier, **Propositus** toggle, **Trait Color** (custom hex picker for affected fill), **Notes** (clinical textarea shown on hover tooltip), and a **Duplicate** action.

### Generation Labelling

Individuals are automatically clustered into generations by vertical proximity (±55 px), sorted left to right, and labelled `II-3`, `III-7` etc. Generation labels on the left margin show Roman numeral + member count, e.g. `II (3)`. All labels update live as individuals are moved.

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&pause=9999&color=007ACC&center=true&vCenter=true&width=600&height=40&lines=%F0%9F%8E%A8+UI+Design" alt="UI Design" />
</div>

### Layout

```
┌─ Title Bar ────────────────────────────────────────────────────┐
│ ● ● ●  [Pedigree] [Punnett Square]   title    Snap Guides … ⬇  │
├────────┬──────────────────────────┬──────────────────────────  │
│ Act.   │ Sidebar                  │ Canvas / Punnett View       │
│ Bar    │ ├─ Tools                 │                             │
│        │ │  ├─ Individuals        │  (infinite canvas)          │
│        │ │  ├─ Relationships      │   or                        │
│        │ │  ├─ History            │  (Punnett grid + ratios)    │
│        │ │  ├─ Selection          │                       [+]   │
│        │ │  ├─ Layout             │                       [⊙]   │
│        │ │  └─ Search / File      │                       [−]   │
│        │ ├─ Properties            │                             │
│        │ ├─ Statistics            │                             │
│        │ └─ Legend                │                             │
├────────┴──────────────────────────┴─────────────────────────── │
│ Status Bar  tool │ count │ selected │ affected │ carriers │ zoom│
└────────────────────────────────────────────────────────────────┘
```

### Colour Palette

| Variable | Hex (dark) | Usage |
|---|---|---|
| `--bg` | `#1e1e1e` | Canvas background |
| `--bg-panel` | `#252526` | Sidebar, actbar |
| `--bg-sidebar` | `#2c2c2c` | Tool / button fills |
| `--bg-titlebar` | `#323233` | Title bar |
| `--bg-sel` | `#04395e` | Selected state fill |
| `--accent` | `#007acc` | Selection, status bar, active borders |
| `--text` | `#cccccc` | Primary text |
| `--text-dim` | `#858585` | Labels, hints |
| `--text-blue` | `#569cd6` | IDs, values, dominant cells |
| `--text-teal` | `#4ec9b0` | Propositus, connection highlight, notes dot |
| `--red` | `#f44747` | Danger, recessive cells |
| `--yellow` | `#dcdcaa` | Section headings, intermediate cells |

Light theme mirrors VS Code Light+ with matching CSS variable overrides via `body.light`.

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&pause=9999&color=4EC9B0&center=true&vCenter=true&width=600&height=40&lines=%E2%8C%A8%EF%B8%8F+Controls" alt="Controls" />
</div>

### Full Keyboard Reference

| Key | Action |
|-----|--------|
| `V` / `Esc` | Select tool / cancel |
| `M` | Place Male |
| `F` | Place Female |
| `U` | Place Unknown |
| `I` | Place Miscarriage |
| `R` | Marriage line |
| `K` | Consanguineous line |
| `C` | Child / descent |
| `T` | Twin lines |
| `Ctrl+Z` | Undo (80-step history) |
| `Ctrl+Y` / `Ctrl+Shift+Z` | Redo |
| `Ctrl+A` | Select all |
| `Ctrl+D` | Duplicate selected |
| `Ctrl+S` | Save JSON |
| `Ctrl+Shift+0` | Zoom to fit all |
| `Ctrl+F` | Zoom to selection |
| `↑ ↓ ← →` | Nudge selected (10 px) |
| `Shift + arrows` | Fine nudge (1 px) |
| `Del` / `Backspace` | Delete selected individual(s) or selected relationship |
| `Space + drag` | Pan canvas (Figma-style) |
| `Ctrl+0` | Reset viewport |
| `Dbl-click` | Inline rename |

### Mouse Controls

| Action | Result |
|--------|--------|
| Click (place tool) | Place individual |
| Click (select tool) | Select individual |
| `Shift+click` | Add/remove from multi-selection |
| Click-drag empty canvas | Rubber-band box selection |
| Click marriage line | Select relationship |
| Drag individual | Move (moves entire selection if grouped) |
| Scroll | Zoom |
| `Alt+drag` or middle-click | Pan |
| `Space+drag` | Pan (Figma-style) |
| Right-click | Context menu |
| Double-click | Inline rename |
| Hover (600 ms) | Notes tooltip |

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&pause=9999&color=CE9178&center=true&vCenter=true&width=600&height=40&lines=%F0%9F%97%82%EF%B8%8F+File+Structure" alt="File Structure" />
</div>

```
rootify.html  (~1700 lines — one file, no dependencies)
│
├── <style>
│   ├── CSS custom properties (dark + light themes)
│   ├── VS Code layout components
│   └── Punnett Square grid + ratio card styles
│
├── HTML structure
│   ├── Title bar (mode tabs, toggles)
│   ├── Activity bar (4 icons)
│   ├── Sidebar (Tools / Properties / Statistics / Legend)
│   ├── Canvas editor (pedigree mode)
│   ├── Punnett view (settings sidebar + grid area)
│   └── Overlays (context menu, tooltip, rename input, hint)
│
└── <script>
    ├── State (S)         Single object — all app state
    ├── History           80-step undo/redo (JSON snapshots)
    ├── Canvas renderer   Guides, relationships, individuals, selection box
    ├── Hit testing       Individuals (circle/square/diamond) + relationship lines
    ├── Multi-select      Set<id>, rubber-band, Ctrl+A, group drag
    ├── Zoom              In/out, fit-all, fit-selection, reset
    ├── Theme             CSS class toggle on body
    ├── Save/Load         JSON serialize/deserialize + FileReader
    ├── Statistics        Live computed panel
    ├── Properties        Dynamic editor with color picker + notes
    ├── Export PNG        Off-screen canvas → PNG download
    └── Punnett Module
        ├── renderMono()   Monohybrid 2×2 grid
        ├── renderDi()     Dihybrid 4×4 grid + gamete generation
        ├── renderXLink()  X-linked 2×2 with preset genotypes
        ├── renderBlood()  ABO blood type cross
        └── makeRatioCard() Genotype + phenotype frequency cards
```

---

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&pause=9999&color=28C840&center=true&vCenter=true&width=600&height=40&lines=%F0%9F%8C%90+Browser+Compatibility" alt="Browser Compatibility" />
</div>

| Browser | Version | Status |
|---------|---------|--------|
| Chrome / Edge | 90+ | ✅ Full support |
| Firefox | 88+ | ✅ Full support |
| Safari | 14+ | ✅ Full support |

---

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&pause=9999&color=007ACC&center=true&vCenter=true&width=700&height=40&lines=%F0%9F%93%96+Version+History" alt="Version History" />

| Version | Highlights |
|---------|-----------|
| **v3.0** | Punnett Square mode, 15 new features, multi-select, light theme, statistics panel, JSON save/load |
| **v2.0** | Undo/redo, snap-to-grid, zoom buttons, miscarriage symbol, auto-arrange, duplicate, nudge keys, guide lines, birth year, notes |
| **v1.0** | Core pedigree editor — all standard symbols, relationship lines, generation labels, context menu, PNG export |

<br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=13&pause=4000&color=858585&center=true&vCenter=true&width=600&height=30&lines=MIT+License+%E2%80%94+free+to+use%2C+modify%2C+and+distribute" alt="license" />

<br/>

**Rootify** — *because every family tree deserves a clean commit history.*

</div>
