# MacroEvoEco Website - Project Guide

## Project Overview
Migrating the Macroevolution and Macroecology Group (ANU) website from Weebly to GitHub Pages using Quarto.

## Current Status
- **Phase**: Iterative design review — scaffold built, content populated, awaiting user feedback
- **Original site**: http://www.macroevoeco.com/ (Weebly, currently offline)
- **Domain**: macroevoeco.com (to be preserved during migration)

## Site Structure
5 pages (matching original + Publications):
1. **Home** (`index.qmd`) - Hero banner, research themes, textbooks, latest pubs, affiliation logos
2. **People** (`people.qmd`) - Leader profiles (Lindell, Marcel) + member card grid
3. **Alumni** (`alumni.qmd`) - Former postdocs, PhDs, RAs with thesis titles
4. **Projects** (`projects.qmd`) - 7 funded research projects with grant details
5. **Publications** (`publications.qmd`) - Chronological list, lab members bolded

## Design
- **Colour palette**: Red desert tones extracted from banner image (P4220620.jpg)
  - Darkest: `#5A2918`, Dark: `#763D24`, Mid: `#C83D11`
  - Warm: `#D4956A`, Light: `#C2AF84`, Cream: `#F5EDE0`
- **Fonts**: Playfair Display (headings), Source Sans Pro (body)
- **Inspired by**: Landis Lab (earth tones, minimal nav) + Keogh Lab (narrative bios, clean layout)

## Build Commands
```bash
# Preview locally (hot reload)
quarto preview

# Build site
quarto render

# Clean + rebuild
rm -rf docs && quarto render
```

## File Structure
```
MacroEvoEco/
├── _quarto.yml        # Site configuration
├── index.qmd          # Home page
├── people.qmd         # People page
├── alumni.qmd         # Alumni page
├── projects.qmd       # Projects page
├── publications.qmd   # Publications page
├── styles.scss        # Custom SCSS styles (main)
├── styles.css         # CSS overrides (minimal)
├── _extensions/       # Quarto extensions (iconify)
├── images/            # Site images
│   ├── banner.jpg           # Red desert hero image
│   ├── textbook-*.jpg       # 3 textbook covers
│   ├── logo-*.{jpg,png}     # ANU, CBA, ECDI logos
│   └── placeholder-person.jpg
└── docs/              # Built site output (GitHub Pages)
```

## Key People
- **Lindell Bromham** - Professor, Evolutionary Biology, ANU. Director of Tempo and Mode.
- **Marcel Cardillo** - Researcher, ANU RSB.
- **Xia Hua** - Researcher, co-investigator on ARC grants.
- **Alex Skeels** - ARC DECRA Fellow (2025-2027).
