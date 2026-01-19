# HaloCSS

HaloCSS is a **utility-first CSS framework** focused on **clean surfaces, subtle depth, and composable UI primitives**.

It’s built to be fast to write, easy to reason about, and flexible enough to scale from demos to real apps.

HaloCSS is a module of the **Orbital** ecosystem, but works perfectly on its own.

---

## What HaloCSS is good at

- Utility-first layout & spacing
- Cards, surfaces, and elevation
- Glass / blur primitives
- Accent colors & glow (optional, controlled)
- Small, readable class names
- Zero JavaScript required

Not a Tailwind clone, not a design system lock-in — just a solid CSS toolkit.

---

## Installation

### CDN (recommended for quick use)

```html
<link
  rel="stylesheet"
  href="https://nightnovann.github.io/HaloCSS/halo.min.css"
/>
```

Unminified (for debugging / learning):

```html
<link rel="stylesheet" href="https://nightnovann.github.io/HaloCSS/halo.css" />
```

---

### Local (Git)

```bash
git clone https://github.com/NightNovaNN/HaloCSS.git
cd HaloCSS
```

Then include it:

```html
<link rel="stylesheet" href="HaloCSS/halo.css" />
```

Or bundle it yourself into `halo.min.css`.

---

## Basic Usage

```html
<body class="pf pf-dark">
  <div class="card card-glass accent-cyan">
    <h2>HaloCSS</h2>
    <p>Glass surface with accent</p>

    <button class="btn btn-solid rc-pill hover-grow">Button</button>
  </div>
</body>
```

---

## Layout & Utilities

```html
<div class="flex justify-between items-center gap-md p-lg">
  <span>Left</span>
  <span>Center</span>
  <span>Right</span>
</div>
```

Common utilities:

- `flex`, `grid`
- `gap-sm / md / lg`
- `p-sm / md / lg`
- `rc-sm / md / pill`
- `justify-*`, `items-*`

---

## Cards & Surfaces

```html
<div class="card">Default</div>
<div class="card card-elevated">Elevated</div>
<div class="card card-flat">Flat</div>
<div class="card card-glass">Glass</div>
```

Optional glow / aura:

```html
<div class="card card-halo accent-blue">Glow</div>
```

Nothing is forced — glow is opt-in.

---

## Buttons

```html
<button class="btn btn-solid">Solid</button>
<button class="btn btn-outline">Outline</button>
<button class="btn btn-ghost">Ghost</button>
```

Sizes & shapes:

```html
btn-sm / btn-md / btn-lg rc-sm / rc-md / rc-pill
```

---

## Animations (CSS-only)

```html
<div class="fade-in">Fade</div>
<div class="slide-up">Slide</div>
<div class="scale-in">Scale</div>
<div class="ping">Ping</div>
```

Hover helpers:

```
hover-grow
hover-lift
```

---

## Themes

Apply on `body` or any container:

```html
<body class="pf pf-dark">
  <div class="pf pf-light"></div>
  <div class="pf pf-code"></div>
  <div class="pf pf-void"></div>
  <div class="pf pf-paper"></div>
</body>
```

Themes are CSS-variable based and override-friendly.

---

## Orbital Ecosystem

HaloCSS is one module under **Orbital**:

```sh
Orbital
 ├─ HaloCSS   (UI & styling)
 ├─ Fractal   (inline image / canvas)
 ├─ AtomCSS   (docs & code styling)
 └─ MDFlow    (markdown rendering)
```

Use HaloCSS alone or combine modules as needed.

---

## Philosophy

- Defaults should be usable
- Effects should be optional
- CSS should stay readable
- No build step required

---

## License

MIT.

Do whatever.

---
