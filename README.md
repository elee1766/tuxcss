# tux.css

classless css. monospaced, lowercase, flat, dense. for dashboards and admin tools.

**[preview](https://elee1766.github.io/tuxcss)**

## install

vendor it. copy the file into your project, change what you want.

```
curl -O https://github.com/elee1766/tuxcss/releases/latest/download/tux.css
curl -O https://github.com/elee1766/tuxcss/releases/latest/download/tux.min.css
```

or link from cdn:

```html
<link rel="stylesheet" href="https://elee1766.github.io/tuxcss/tux.min.css">
```

sri hashes for both files are on the [preview page](https://elee1766.github.io/tuxcss) and auto-generated on each build.

## what it styles

plain html elements. no classes.

- `section`, `article`, `aside` -- bordered cards with header bars
- `table` -- muted headers, row borders, hover
- `button` -- primary/soft/danger/ghost via `data-variant`
- `details` -- accordion
- `dialog` -- modal
- `progress`, `meter` -- bars
- `[data-alert]` -- info/success/warning/error banners
- `[data-grid="2|3|4"]` -- grid layout

colors are `--tux-*` custom properties. override them.

## font

tux.css uses Cousine as the primary font, with fallbacks to other monospace fonts. no font files are bundled. if you want Cousine, add this before tux.css:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Cousine:ital,wght@0,400;0,700;1,400;1,700&display=swap">
```

without it, the browser picks the next available monospace font from the stack: JetBrains Mono, IBM Plex Mono, Fira Code, Source Code Pro, or the system default.

## dark mode

auto-adapts to `prefers-color-scheme`. to override manually:

```html
<html data-theme="dark">
<html data-theme="light">
```

omit `data-theme` to follow system preference.

## license

MIT
