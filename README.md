# Keepsake — Responsive Landing Page

Responsive one-page landing based on the Keepsake Figma design (Desktop 1280, Tablet 768, Mobile 375, Mobile menu open, UI states).

## Demo

[Live Demo — Keepsake](https://demianmysiv.github.io/landing-keepsake/)

## Technologies and decisions

- HTML5 semantic layout (`header`, `nav`, `main`, `section`, `article`, `footer`, `form`).
- CSS mobile-first (base mobile, breakpoints at 768px and 1280px), Flexbox and Grid.
- CSS design tokens (`:root`), Google Fonts (Oswald, Open Sans, Dancing Script).
- WebP assets in `images/`, inline SVG icons, lazy loading of below-the-fold images.
- Portfolio filters with `:checked ~` radio input sibling selectors (no JavaScript).
- Mobile menu with the native HTML Popover API and button `popovertarget` (no JavaScript).
- Form uses native email and required-checkbox validation; successful valid submission navigates to a local `#newsletter-success` demo state; no email is delivered or saved.

## Project structure

```
landing-keepsake/
  index.html
  css/style.css
  images/           (copy your supplied 19 WebP image files here)
  fonts/            (optional; Google Fonts are loaded over the network)
```

## Verify

1. Preview `index.html` with an HTTP server (e.g. VS Code Live Server).
2. Check responsive widths 320, 375, 768, 1280 and 1920 px.
3. Test keyboard access (Tab, Enter, Space, Escape), filter categories, the burger/close state, email validity and consent.
4. Test current Chrome, Firefox and Edge.
5. Validate `index.html` with https://validator.w3.org/ .

Note: social links, favourites, journal articles and LOAD MORE are visual elements of the given static layout; there is no backend or additional project content supplied. These do not implement live services.
