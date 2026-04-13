# Reports — Played Data Dashboards

## Overview
Interactive HTML-based commissioning and participation reports. Zero-infrastructure static dashboards generated from club-enrichment data. Currently two reports: Short Breaks (Norfolk County Council) and Get into Golf (England Golf).

## Stack
- Pure HTML/CSS/JavaScript (no build tools, no framework)
- Chart.js v4.4.7 for data visualisation
- Plus Jakarta Sans font (Google Fonts CDN)
- Single-file, self-contained reports (~40-50KB each)

## Files
```
short-breaks.html    # Norfolk children's SEND services dashboard
get-into-golf.html   # England Golf participation analysis
```

## Design
- Dark theme (#1C1C1E background)
- Primary: coral #E85D6C
- CSS custom properties for theming
- Responsive (breakpoints: 600px, 900px)
- Print stylesheet for PDF export
- Scroll-triggered fade-in animations
- Animated number counters

## Features
- Tab-based chart switching with lazy initialisation
- Date range filtering (YTD, quarterly, custom)
- Chart.js bar, line, doughnut charts
- Intersection Observer for scroll animations
- No external dependencies beyond CDN Chart.js + Google Fonts

## Notes
- Data is hardcoded in JavaScript objects within each HTML file
- Reports are generated from club-enrichment pipeline data
- Identical copies exist in the club-enrichment repo
- Template pattern: same HTML structure, different data — could be formalised
