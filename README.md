# Brandeez v2 — Responsive Landing Page

A redesign of the original [brandeez-elevate](https://github.com/uditplayz/brandeez-elevate) landing page, converted into a polished, mobile-friendly layout using **CSS media queries**.

## What changed from v1
- New dark visual theme (Space Grotesk + Inter), gradient accents, and a CSS-only browser mock-up in place of the hotlinked photo.
- New sections: stats strip, services cards, selected-work grid, about, and a full-width contact CTA.
- Accessible mobile menu: a real `<button>` with `aria-expanded`, closes on link click / `Esc`, plus a skip link and visible focus states.
- Fixed v1 issues: the contact button's `mailto:` now matches the displayed address, and the footer copyright now says Brandeez.

## Responsive approach
| Breakpoint | Changes |
|---|---|
| `max-width: 768px` | Hero, about and card grids stack to one column; stats become 2×2; work grid becomes a single column; nav collapses into a full-screen hamburger menu; section spacing and type are reduced |
| `max-width: 480px` | Tighter gutters, smaller headline, full-width stacked buttons, smaller stat numbers |

Other techniques: viewport meta tag, fluid type with `clamp()`, relative units (`rem`, `%`), Flexbox + CSS Grid, `max-width: 100%` images/SVGs, `overflow-x` guard, and `prefers-reduced-motion` support.

## Testing
Checked in Chromium at 1280, 768, 375 and 320 px widths: no horizontal overflow at any size, and the mobile menu opens and closes correctly.

## Files
- `index.html` — structure and content (plus a few lines of JS for the menu)
- `style.css` — design tokens, layout, and media queries

Open `index.html` in a browser and resize the window (or use the Chrome DevTools device toolbar) to see it adapt.
