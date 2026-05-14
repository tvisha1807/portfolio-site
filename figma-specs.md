# Figma Specs — Landing Page (node 302:2603 → 303:2731)

> Extracted from Figma file `bfFd7bco53GPbSk1TxHLCF`, page "New ", frame "Landing Page" (`303:2731`).
> Frame dimensions: **1728 × 3967 px** (desktop only — no tablet/mobile breakpoints defined in this file).

---

## 1. Section inventory (top → bottom)

| # | Section | Node ID | Y offset | Size (w × h) | Visible |
|---|---------|---------|----------|---------------|---------|
| 1 | **Hero** (header + intro + decorative blobs) | `699:6896` | 58 | 1633 × 817 | Yes |
| 2 | **Projects label** ("Projects / Recently I made,") | `484:7562` | 951 | 1510 × 84 | Yes |
| 3 | **Projects container** (3 visible case-study cards) | `443:5487` | 1081 | 1512 × 2759 | Yes |
| — | Decorative background vectors (blobs) | `488:5788`, `488:5789` | 2978 / 3849 | ~766 × 766 each | Yes |
| — | Appreciations section (hidden) | `391:5855` | 3825 | 1510 × 84 | **No** |
| — | Project 4 – eye-appointment (hidden) | `370:4887` | 3016 | 1512 × 1210 | **No** |

### 1a. Hero breakdown (`699:6896`)

- **Decorative vectors** (abstract blob shapes, purple/pink gradient fills):
  - Left blob `484:7567` — 547 × 537 at (0, 176)
  - Right blob `484:7569` — 766 × 766 at (1633, 640), rotated 134.45°
- **Header** (`699:6893`, y=0, 1591 × 36):
  - Logo frame `535:6688` → text "tvisha " (Poppins Bold 24px, black)
  - Decorative line `535:6687` — 62px wide, centered
  - Nav links `699:6894` → "work" + "about me" (Poppins Bold 24px, black, 16px gap)
- **Hero text** (`303:2749` "About me", y=264):
  - Greeting: "Hi! I am Tvisha" — Poppins Regular 36px, black
  - Headline: "I am a product designer with a Bachelors in Industrial Design. I work towards creating **simple and inclusive user experiences.**" — Poppins Bold 64px, black with accent span in **#9D02FC** (purple)

### 1b. Projects section label (`484:7562`)

- "Projects" — 30px (appears to be a small label/overline)
- "Recently I made," — 54px (section heading)

### 1c. Project cards (`443:5487` → `370:4885`)

Inner container has 8px padding.

#### Project 1 — full width (`336:2620`, 1504 × 1203)

- **Title** (`336:2622`): "Foundations for a scalable design system with MUI integration for a global financial institution"
- **Link** (`336:2625`): "Click to view the project↗"
- **Image area** (`377:5999`, 1504 × 952): Contains a "Material 3 Design Kit" cover illustration (left side, ~851 × 479) and a data table UI screenshot (right side, ~653 × 648). This is a composite illustration, not a simple photo.

#### Project 2 — two columns (`336:2603`, 1511 × 682, y=1291)

- **Left text** (`336:2604`, 743 × 458):
  - Title: "A portal for resource management, allowing efficient resource tracking and quicker deployment"
  - Description: "Combining the ease of e-commerce while still retaining the authentic experience of thrifting."
  - Link: "Click to view the project↗"
- **Right image** (`376:6304`, 744 × 682): Honeycomb-pattern resource management interface mockup

#### Project 3 — two columns (`443:5479`, 1506 × 682, y=2061)

- **Left text** (`443:5480`, 743 × 458):
  - Title: "An efficient way to onboard new employees"
  - Description: "Starting a new job is stressful enough, onboarding shouldn't add to that. We worked on streamlining the onboarding journey to create a better experience for new joinees."
  - Link: "Click to view the project↗"
- **Right image** (`443:5485`, 744 × 682): Employee onboarding app screens

---

## 2. Typography

| Token | Family | Weight/Style | Size | Line-height | Usage |
|-------|--------|-------------|------|-------------|-------|
| `nav` | Poppins | Bold | 24px | normal | Header logo "tvisha", nav links |
| `greeting` | Poppins | Regular | 36px | normal | "Hi! I am Tvisha" |
| `hero-headline` | Poppins | Bold | 64px | normal | Hero intro paragraph |
| `section-label` | Poppins | (tbd) | 30px | normal | "Projects" overline |
| `section-heading` | Poppins | (tbd) | 54px | normal | "Recently I made," |
| `project-title` | Poppins | (tbd) | ~48px | normal | Case study titles (large text, ~144px height for 3 lines) |
| `project-desc` | Poppins | (tbd) | ~24px | normal | Case study descriptions |
| `project-link` | Poppins | (tbd) | 24px | normal | "Click to view the project↗" |

**Font family**: **Poppins** throughout (replaces the placeholder Inter + Fraunces in current `global.css`).

---

## 3. Color palette

| Token | Value | Usage |
|-------|-------|-------|
| `--color-text` | `#000000` (black) | All body/heading text |
| `--color-accent` | `#9D02FC` | Highlighted hero text "simple and inclusive user experiences." |
| `--color-bg` | `#FFFFFF` (white) | Page background |
| `--color-blob` | `#ECCCFF` (light lavender) | Decorative hero & footer blobs (blurred organic SVG shapes) |
| `--color-link-underline` | `#9D02FC` (likely) | "Click to view the project↗" links |
| `--color-nav-line` | `#000000` (black) | Small decorative horizontal line in header |

---

## 4. Layout & spacing

| Property | Value |
|----------|-------|
| Design width | 1728px |
| Side padding (page) | ~108px (content starts at x≈108) |
| Content max-width | ~1512px |
| Hero area content inset | ~35–43px additional from frame edge |
| Projects container padding | 8px inner |
| Gap between project cards | ~88px (Project 1 ends at y≈1203, Project 2 starts at y≈1291) |
| Nav gap between links | 16px |
| Section label → heading gap | 0 (stacked, label 30px + heading 54px = 84px total) |
| Hero greeting → headline gap | ~(-4px) overlapping (tight stack) |

---

## 5. Breakpoints

**Only desktop (1728px)** is defined in this Figma frame. No responsive variants (tablet, mobile) were found in the inspected node tree. Responsive behavior will need to be designed during implementation using sensible defaults.

---

## 6. Assets to export

| Asset | Node ID(s) | Type | Notes |
|-------|-----------|------|-------|
| Hero blob (left) | `484:7567` | SVG vector | Purple/pink gradient, ~547×537 |
| Hero blob (right) | `484:7569` | SVG vector | Same style, ~766×766, rotated 134.45° |
| Footer blob 1 | `488:5788` | SVG vector | ~766×766 |
| Footer blob 2 | `488:5789` | SVG vector | ~766×766 |
| Nav decorative line | `535:6687` | SVG/CSS | 62px horizontal line |
| Project 1 cover image | `377:5999` | Raster (PNG) | Material 3 Design Kit composite, 1504×952 |
| Project 2 image | `376:6304` + children | Raster (PNG) | Honeycomb resource portal, 744×682 |
| Project 3 image | `443:5485` + children | Raster (PNG) | Onboarding app screens, 744×682 |

### Downloaded assets (in `public/assets/`)

| File | Description | Key details |
|------|-------------|-------------|
| `hero-blob-left.svg` | Blurred organic shape | Fill: `#ECCCFF`, Gaussian blur σ=158, viewBox 1179×1169 |
| `hero-blob-right.svg` | Same shape, positioned differently | Fill: `#ECCCFF`, Gaussian blur σ=158 (rotated 134.45° in layout) |
| `nav-line.svg` | Thin horizontal line | 62px wide, black stroke |

**Still needed** (Figma rate limit hit before export):
- Project 1 composite image (Material 3 Design Kit cover + data table) — node `377:5999`
- Project 2 image (honeycomb resource portal) — node `376:6304`
- Project 3 image (onboarding screens) — node `443:5485`
- Footer decorative blobs — nodes `488:5788`, `488:5789` (same shape as hero blobs, can reuse)

---

## 7. Component inventory (repeating patterns)

| Pattern | Count | Where |
|---------|-------|-------|
| **Header** (logo + line + nav) | 1 | Top of hero; reusable across pages |
| **Project card — full width** | 1 | Project 1 (title + link + full-width image) |
| **Project card — split** (text left, image right) | 2 | Projects 2 & 3 (title + desc + link | image) |
| **Section label + heading** | 1 | "Projects / Recently I made," |
| **Decorative blob** | 4 | 2 in hero, 2 near footer |

---

## 8. Mapping to existing codebase

| Figma element | Current file | Action needed |
|---------------|-------------|---------------|
| Font: Poppins | `global.css` `--font-sans: Inter` | Replace Inter with Poppins; drop Fraunces |
| Brand colors | `global.css` `--color-brand-*` | Replace entire palette with `--color-accent: #9D02FC`, simplify |
| Header/nav | Not present in `BaseLayout.astro` | Create `Header.astro` component, add to layout |
| Hero section | `index.astro` basic hero | Rewrite with Figma copy, accent styling, blob backgrounds |
| Project cards | `index.astro` grid from `getCollection` | Restructure: 1 full-width + 2 split cards; keep data-driven approach |
| Footer | Not in Figma landing | None for now |

---

## 9. Reference screenshots

- **Full landing page** (1728×3967): captured via `get_screenshot` node `303:2731` — shows complete vertical flow from header through all 3 project cards.
- **Hero section code** was obtained via `get_design_context` on `699:6896` — provides exact layout, font specs, and asset URLs.
