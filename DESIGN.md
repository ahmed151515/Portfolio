---
name: Sys.Ahmed Design System
description: Expert, clean, modern backend portfolio
colors:
  primary: "oklch(0.65 0.25 25)"
  primary-hover: "oklch(0.75 0.25 25)"
  primary-wash: "oklch(0.15 0.05 25)"
  bg: "oklch(0.05 0 0)"
  surface: "oklch(0.12 0 0)"
  surface-border: "oklch(0.25 0 0)"
  ink: "oklch(0.98 0 0)"
  muted: "oklch(0.60 0 0)"
typography:
  display:
    fontFamily: '"Archivo", sans-serif'
    fontSize: "clamp(2rem, 5vw, 3.5rem)"
    fontWeight: 700
  hero:
    fontFamily: '"Archivo", sans-serif'
    fontSize: "clamp(3rem, 8vw, 6rem)"
    fontWeight: 700
  body:
    fontFamily: '"Archivo", sans-serif'
    fontSize: "1rem"
    lineHeight: 1.65
  label:
    fontFamily: '"JetBrains Mono", monospace'
    fontSize: "0.875rem"
    fontWeight: 700
    letterSpacing: "0.1em"
rounded:
  sm: "2px"
  md: "4px"
  full: "9999px"
spacing:
  1: "0.25rem"
  2: "0.5rem"
  3: "0.75rem"
  4: "1rem"
  5: "1.25rem"
  6: "1.5rem"
  8: "2rem"
  10: "2.5rem"
  12: "3rem"
  16: "4rem"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.ink}"
    rounded: "{rounded.sm}"
    padding: "0.75rem 1.5rem"
  button-default:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.sm}"
    padding: "0.75rem 1.5rem"
---

# Design System: Sys.Ahmed

## 1. Overview

**Creative North Star: "The Cyber-Engineer"**

This visual system evokes the precision, raw power, and absolute reliability of high-level backend engineering. It leans on a cyber-brutalist aesthetic—stark voids, monospace typography, and warning-red accents—to demonstrate technical expertise without generic templates or cartoonish distraction. The layout is disciplined, treating the screen as a terminal interface composed of high-precision structural units.

We explicitly reject cluttered layouts, generic Bootstrap/Tailwind aesthetics, and anything overly playful or un-structured.

**Key Characteristics:**
- **Expert Confidence:** Unapologetic contrast and rigid grid structures.
- **Show, Don't Tell:** Sharp micro-interactions and precision alignments.
- **Clarity Over Clutter:** Absolute minimal distraction; if it's not data, it's black.

## 2. Colors

The Cyber-Brutalist palette is an exercise in restraint and high contrast, grounded in void-black and stark white, punctuated by a single intense accent.

### Primary
- **Cyber Warning Red** (oklch(0.65 0.25 25)): Used strictly for high-priority actions, terminal-like typing accents, and hover states. 
- **Cyber Warning Wash** (oklch(0.15 0.05 25)): Used as a subtle indicator background for technical badges.

### Neutral
- **Pure Void** (oklch(0.05 0 0)): The base background. Absolute depth.
- **Deep Panel** (oklch(0.12 0 0)): Surface backgrounds for structural containers.
- **Stark Border** (oklch(0.25 0 0)): Borders mapping out the grid.
- **Stark Ink** (oklch(0.98 0 0)): Primary text and sharp highlights.
- **Muted Data** (oklch(0.60 0 0)): Secondary text, descriptions, and passive timestamps.

**The One Voice Rule.** The primary accent is used on ≤10% of any given screen. Its rarity is what gives it warning-level power.

## 3. Typography

**Display Font:** Archivo (sans-serif)
**Body Font:** Archivo (sans-serif)
**Label/Mono Font:** JetBrains Mono (monospace)

**Character:** Archivo provides brutalist, geometric authority, while JetBrains Mono injects the raw feel of an IDE terminal.

### Hierarchy
- **Hero** (700, clamp(3rem, 8vw, 6rem), 1.05): The unignorable page title.
- **Display** (700, clamp(2rem, 5vw, 3.5rem), 1.2): Primary section headers.
- **Title** (700, clamp(1.5rem, 3vw, 2rem), 1.2): Component and card titles.
- **Body** (400, 1rem, 1.65): Standard prose and descriptions. Max 65ch width.
- **Label** (700, 0.875rem, uppercase, 0.1em spacing): Terminal-style eyebrows and badges.

**The Terminal Rule.** Monospace is strictly reserved for data (dates, code), interactive labels, and terminal-flavor accents. Never for body paragraphs.

## 4. Elevation

Stark flat planes with sharp geometric borders, zero shadow.

### Named Rules
**The Void Rule.** The Z-axis is flat. Depth is conveyed entirely through high-contrast borders separating deep panels from the void background. No box-shadows, ever.

## 5. Components

High-precision structural units, solid and unyielding.

### Buttons
- **Shape:** 2px radius (sharp precision)
- **Primary:** Cyber Warning Red background, stark ink text, 0.75rem 1.5rem padding.
- **Hover / Focus:** Shifts to a brighter Warning Red (oklch(0.75 0.25 25)).
- **Secondary / Ghost / Tertiary (if applicable):** Transparent background with stark border, turning to deep panel on hover.

### Cards / Containers
- **Corner Style:** 2px radius
- **Background:** Deep panel
- **Shadow Strategy:** Zero shadow (Void Rule)
- **Border:** 1px stark border
- **Internal Padding:** 2rem scale

### Inputs / Fields
- **Style:** 1px stark border, transparent background, 2px radius.
- **Focus:** Border turns Cyber Warning Red.

### Navigation
- **Style:** Flat top nav, transparent to pure void background on scroll, stark bottom border.

## 6. Do's and Don'ts

### Do:
- **Do** use strict monochromatic structures with stark borders to define space.
- **Do** employ monospace fonts for technical data, tags, and small utility text.
- **Do** keep animations sharp and purposeful (e.g. blink cursors, stark hover snaps).

### Don't:
- **Don't** use generic Bootstrap/Tailwind templates or overly playful aesthetics.
- **Don't** clutter layouts; maintain empty void space for visual relief.
- **Don't** use drop shadows (box-shadow) or glassmorphism to show elevation.
- **Don't** use border-radius greater than 4px on any structural element.
