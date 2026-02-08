# Usage Guide

<!--
  © 2026 RSK World | https://rskworld.in
  Founder: Molla Samser
  Email: help@rskworld.in | support@rskworld.in
  Phone: +91 93305 39277
  Address: Nutanhat, Mongolkote, Purba Burdwan, West Bengal, India, 713147
-->

Quick guide to using the Responsive Design System in your project.

## 1. Include the stylesheet

```html
<link rel="stylesheet" href="path/to/css/design-system.css">
```

Or link individual files if you need a smaller bundle (e.g. only tokens + grid + utilities).

## 2. Basic layout

```html
<div class="rsk-container">
  <div class="rsk-row" style="--rsk-gutter-x: 1rem;">
    <div class="rsk-col rsk-col-12 rsk-col-md-6">Column A</div>
    <div class="rsk-col rsk-col-12 rsk-col-md-6">Column B</div>
  </div>
</div>
```

## 3. Components

- **Button:** `class="rsk-btn rsk-btn-primary"` (or `rsk-btn-secondary`, `rsk-btn-outline-primary`, `rsk-btn-sm`, `rsk-btn-lg`).
- **Card:** `class="rsk-card"` with optional `rsk-card-header`, `rsk-card-body`, `rsk-card-footer`.
- **Alert:** `class="rsk-alert rsk-alert-info"` (or success, warning, danger).
- **Input:** `class="rsk-input"` with `class="rsk-label"` on the label.

## 4. Theme (dark/light)

Set on the root element:

```html
<html data-theme="dark">
```

Or use JavaScript to toggle and optionally store in `localStorage` (see `components.html`).

## 5. Overriding tokens

In your own CSS (after the design system):

```css
:root {
  --rsk-color-primary: #your-brand-color;
  --rsk-radius-lg: 0.75rem;
}
```

## 6. Advanced components (modal, tabs, dropdown)

These need a small script for open/close and ARIA. Copy the script from `components.html` or implement your own using the same class names (e.g. `.is-open`, `aria-expanded`, `aria-hidden`).

## 7. Print

Print styles are included. Use `class="rsk-no-print"` to hide elements when printing.

## 8. Accessibility

- Use the skip link: `<a href="#main" class="rsk-skip-link">Skip to main content</a>`.
- Focus styles use `:focus-visible`. Keep interactive elements keyboard-accessible.
- Respect `prefers-reduced-motion` (animations are disabled when requested).

## More

- **Full docs:** Open `documentation.html` in a browser.
- **Examples:** See `examples.html` and `components.html`.
- **File list:** See README.md “File structure”.

---

**RSK World** · https://rskworld.in · help@rskworld.in · +91 93305 39277
