# tux.css

classless css for terminal-style interfaces. monospaced, lowercase, no rounded corners, no shadows.

**[preview](https://elee1766.github.io/tuxcss)**

## usage

the best way to use tux.css is to vendor it -- copy `tux.css` into your project and modify it to fit. the file is self-contained with no dependencies.

```
curl -O https://github.com/elee1766/tuxcss/releases/latest/download/tux.css
```

or the minified version:

```
curl -O https://github.com/elee1766/tuxcss/releases/latest/download/tux.min.css
```

alternatively, link it directly (not recommended for production):

```html
<link rel="stylesheet" href="https://elee1766.github.io/tuxcss/tux.css">
```

## what it does

styles semantic html elements directly. no classes needed. write `<section>`, `<table>`, `<button>`, `<details>` etc. and it looks right.

- `<section>`, `<article>`, `<aside>` become bordered cards with optional `<header>` bars
- `<table>` gets muted header rows, subtle row borders, hover states
- `<button>` has 4 variants via `data-variant`: primary (default), soft, danger, ghost
- `<details>` becomes an accordion with expand indicators
- `<dialog>` becomes a modal
- `<progress>` and `<meter>` are styled
- `[data-alert]` on any element makes it an alert (info, success, warning, error)
- `[data-grid="2|3|4"]` gives you a simple grid

all colors are exposed as `--tux-*` css custom properties for easy overriding.

## license

MIT
