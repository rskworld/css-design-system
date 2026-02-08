# Responsive Design System

<!--
  © 2026 RSK World | https://rskworld.in
  Founder: Molla Samser
  Email: help@rskworld.in | support@rskworld.in
  Phone: +91 93305 39277
  Address: Nutanhat, Mongolkote, Purba Burdwan, West Bengal, India, 713147
-->

A comprehensive CSS design system with reusable components, utility classes, design tokens, grid system, themes, animations, and responsive patterns. Minimal JS only for interactive components (modal, tabs, dropdown, accordion, theme toggle).

## Features

- **Component library** – Buttons, cards, badges, alerts, form inputs, nav, list group
- **Advanced components** – Modal, tabs, dropdown, tooltip, breadcrumb, pagination, accordion
- **Typography** – Headings (h1–h6), lead, blockquote, code/pre, kbd, lists, dl-inline
- **Layout** – Stack, cluster, with-sidebar, split, center, flow, region, wrapper, box
- **Forms advanced** – Form group, checkbox/radio, switch (toggle), input group with addon, validation states
- **Tables** – Styled table, striped, bordered, compact, responsive wrapper
- **Effects** – Progress bar, avatar (and group), divider, spinner, empty state, card-img-top, blur
- **Callouts** – Info, success, warning, danger callout boxes with optional icon and title
- **Scroll** – Scroll-snap (x/y), thin/hide scrollbar, scroll-margin for fixed header, smooth scroll
- **Timeline & steps** – Vertical timeline, horizontal stepper (active/done states)
- **Overlays** – Card overlay (image + caption), hero overlay, backdrop, media caption
- **Selection & sticky** – Custom ::selection, sticky-top/bottom, z-index scale
- **Design tokens** – Colors, typography, spacing, radius, shadows, breakpoints (CSS custom properties)
- **Themes** – Light/dark theme via `data-theme`, semantic surface/text tokens, `prefers-color-scheme` support
- **Animations** – Keyframes (fade-in, slide-up, scale-in, spin, pulse, bounce), transition utilities, skeleton loader; respects `prefers-reduced-motion`
- **Grid system** – 12-column flexbox grid with responsive column classes
- **Utility classes** – Display, flex, spacing, text, visibility, border, shadow
- **Focus & a11y** – `:focus-visible` ring, skip link
- **Print styles** – Print-optimized rules in `print.css`
- **Documentation** – In-repo docs and demo pages (index, components, examples, documentation)
- **Responsive patterns** – Visibility by breakpoint, responsive grid, stack/row, reduced motion

## Technologies

- CSS3, CSS Grid, Flexbox, Custom Properties, Component Architecture, Design Tokens

## File structure

```
css-design-system/
├── css/
│   ├── tokens.css             # Design tokens
│   ├── themes.css             # Light/dark theme (data-theme)
│   ├── grid.css               # Grid system
│   ├── utilities.css          # Utility classes
│   ├── typography.css         # Headings, lead, blockquote, code, lists, kbd
│   ├── layout.css             # Stack, cluster, sidebar, split, center, flow, region
│   ├── components.css         # Base components (buttons, cards, badges, etc.)
│   ├── components-advanced.css # Modal, tabs, dropdown, tooltip, breadcrumb, pagination, accordion
│   ├── forms-advanced.css     # Checkbox, radio, switch, input group, validation
│   ├── tables.css             # Table, striped, bordered, compact, responsive
│   ├── effects.css            # Progress, avatar, divider, spinner, empty state, blur
│   ├── callouts.css            # Info, success, warning, danger callouts
│   ├── scroll.css              # Scroll-snap, scrollbar, scroll-margin
│   ├── timeline.css            # Vertical timeline, horizontal stepper
│   ├── overlays.css            # Card overlay, hero overlay, backdrop
│   ├── selection.css           # ::selection, sticky, z-index scale
│   ├── animations.css         # Keyframes, animation/transition utilities, skeleton
│   ├── focus.css              # Focus-visible, skip link
│   ├── responsive.css         # Responsive patterns
│   ├── print.css              # Print styles
│   └── design-system.css      # Main entry (imports all)
├── index.html                 # Demo home
├── components.html            # Advanced components (theme, tabs, modal, etc.)
├── examples.html              # Typography, forms, tables, layout, effects
├── documentation.html        # Documentation
└── README.md
```

## Usage

1. Link the main stylesheet:

```html
<link rel="stylesheet" href="css/design-system.css">
```

2. Use container and grid:

```html
<div class="rsk-container">
  <div class="rsk-row">
    <div class="rsk-col rsk-col-12 rsk-col-md-6">Column 1</div>
    <div class="rsk-col rsk-col-12 rsk-col-md-6">Column 2</div>
  </div>
</div>
```

3. Use components (e.g. button, card):

```html
<button type="button" class="rsk-btn rsk-btn-primary">Primary</button>
<div class="rsk-card">
  <div class="rsk-card-body">Content</div>
</div>
```

4. Override tokens in your CSS if needed:

```css
:root {
  --rsk-color-primary: #your-color;
}
```

5. Enable dark theme: set `data-theme="dark"` on `<html>` (or use the theme dropdown in `components.html`; choice is stored in `localStorage`).

6. Advanced components (modal, tabs, dropdown, accordion) need a small script for open/close and ARIA; see `components.html` for the included script.

## Documentation & license

| File | Description |
|------|-------------|
| [README.md](README.md) | This file – overview, features, usage |
| [USAGE.md](USAGE.md) | Short usage guide |
| [CHANGELOG.md](CHANGELOG.md) | Version history |
| [CONTRIBUTING.md](CONTRIBUTING.md) | How to contribute |
| [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) | Community standards |
| [SECURITY.md](SECURITY.md) | Reporting vulnerabilities |
| [DESIGN-TOKENS.md](DESIGN-TOKENS.md) | Token reference |
| [COMPONENTS.md](COMPONENTS.md) | Component class reference |
| [LICENSE](LICENSE) | MIT License |

## Author & contact

- **RSK World** – [https://rskworld.in](https://rskworld.in)
- **Founder:** Molla Samser
- **Email:** help@rskworld.in | support@rskworld.in
- **Phone:** +91 93305 39277
- **Address:** Nutanhat, Mongolkote, Purba Burdwan, West Bengal, India, 713147

© 2026 RSK World. All rights reserved.
