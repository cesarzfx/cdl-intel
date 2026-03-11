# cdl-intel

A multi-page fan site covering the 2025-26 Call of Duty League season. Built as a mid-term web design project demonstrating responsive layout, advanced CSS techniques, and interactive UI.

## Live Site

You can view the live website here:  
👉 https://cesarzfx.github.io/cdl-intel/

---

## Technologies Used

- HTML5
- CSS3 (compiled from LESS)
- LESS Preprocessor
- Flexbox
- Advanced CSS Selectors
- Font Awesome 6
- GitHub
- GitHub Pages

---

## Project Structure

```
cdl-intel/
├── index.html          — Home page (about CDL, season snapshot, quick links)
├── teams.html          — Teams page (12 flip cards with full rosters)
├── events.html         — Events page (5 major event cards + prediction form)
├── predictions.html    — Predictions page (standalone fan prediction form)
├── favicon.ico         — Custom site favicon
├── css/
│   └── main.css        — Compiled stylesheet
├── less/
│   ├── main.less       — Entry point — imports all partials in order
│   ├── variables.less  — Global colour, font, spacing, and sizing tokens
│   ├── base.less       — Reset, typography, footer, section bands
│   ├── nav.less        — Navigation, hamburger menu, mobile panel
│   ├── cards.less      — Flip cards, teams grid, roster styles
│   ├── events.less     — Event cards, prediction form, form reveal
│   └── responsive.less — All media queries (tablet 768px, mobile 480px)
├── images/
│   └── events/         
├── planning/
│   ├── ContentIntegration.pdf       
│   ├── TopicOutline.pdf  
│   └── Wireframes.pdf       
└── README.md           — Project documentation
```

---

## Week-by-Week Coverage

| Week | Topic | Implementation |
|------|-------|----------------|
| 1 | GitHub & GitHub Pages | Site version-controlled and deployed live via GitHub Pages |
| 2 | Flexbox | Primary layout system — used in teams grid, events grid, about cards, snapshot stats, quicklinks, and form rows |
| 3 | Advanced CSS Selectors | `:checked ~ ` sibling selectors power flip cards, hamburger swap, and form reveal; compound selectors handle per-team card colours; `li:last-child` removes trailing borders |
| 4 | Flip Cards | 12 pure CSS flip cards using hidden checkboxes, `transform-style: preserve-3d`, and `rotateY(180deg)` |
| 5 | Forms | Prediction form with text inputs, radio buttons, grouped `<select>` dropdowns via `<optgroup>`, and a submit button |
| 6 | Favicon, Font Awesome & Hamburger | Custom favicon on all pages; Font Awesome icons throughout; pure CSS hamburger that swaps `fa-bars` → `fa-xmark` on toggle |
| 7 | LESS Preprocessor | 6-file LESS architecture with variables, nesting, and `@import` — compiled to a single `main.css` |

---

## Key CSS Concepts Demonstrated

- Responsive layout with Flexbox and media queries
- 3D card transforms using `perspective`, `transform-style: preserve-3d`, and `rotateY()`
- State-based interactivity with `:checked` and sibling combinators (`~`, `+`)
- Pure CSS show/hide patterns (hamburger menu, form reveal, flip cards)
- LESS variables, nesting, and multi-file architecture
- CSS custom transitions and hover animations
- Sticky navigation with `position: sticky`
- Mobile-first responsive breakpoints at 768px and 480px

---

## Notes

All interactive features — flip cards, hamburger menu, form reveal — are implemented using pure CSS, demonstrating advanced selector and state-based styling techniques. The LESS source files in `/less/` should be compiled using a LESS compiler to regenerate `css/main.css` after any changes.