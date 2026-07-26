# WebDev-L1-TemperatureConverter — Praneeth Madduri

**Track:** Web Development & Designing
**Level:** Level 1 — Task 3
**Task:** Temperature Converter Website

## Overview

An interactive temperature converter that converts a value between Celsius, Fahrenheit, and Kelvin. Each unit has a consistent color across the selector and results, and a live thermometer bar gives instant visual feedback based on the entered value.

## Tech Stack

- HTML5
- CSS3 (Flexbox + Grid, custom properties for theming)
- JavaScript (Vanilla — no libraries or frameworks)
- Google Fonts: Space Grotesk (display), Inter (body), IBM Plex Mono (labels)

## Features

- Numeric input field with custom regex-based validation — rejects non-numeric input with a clear error message instead of silently failing
- Unit selector (Celsius / Fahrenheit / Kelvin) as color-coded segmented radio buttons
- All three converted values shown simultaneously after conversion — no need to pick an output unit separately
- Convert button (also triggers on Enter key)
- Result cards labeled and color-matched to their unit
- Absolute zero edge case handling: any input that converts to below −273.15°C shows a friendly explanatory message instead of an invalid result
- Live thermometer visual that fills based on the parsed temperature
- Clean, centered, single-card layout, responsive down to small mobile widths

## How the Conversion Works

All conversions are normalized through Celsius first:

- **Fahrenheit → Celsius:** `(F − 32) × 5/9`
- **Kelvin → Celsius:** `K − 273.15`
- **Celsius → Fahrenheit:** `C × 9/5 + 32`
- **Celsius → Kelvin:** `C + 273.15`

This keeps a single source of truth for the formulas rather than converting directly between every pair of units.

## File Structure

```
WebDev-L1-TemperatureConverter/
├── index.html      # Complete single-file converter (HTML + inline CSS + JS)
├── README.md        # This file
└── screenshots/     # Add screenshots here before pushing
```

## How to Run

Open `index.html` directly in any modern browser — no build step or server required.

## Author

Praneeth Madduri — Information Science & Engineering Undergraduate, Malnad College of Engineering
praneethmadduri20006@gmail.com · github.com/praneethm · linkedin.com/in/praneethm
