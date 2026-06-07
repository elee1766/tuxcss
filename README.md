# tux.css

classless css. monospaced, lowercase, flat, dense. for dashboards and admin tools.

**[preview](https://elee1766.github.io/tuxcss)**

## install

vendor it. copy the file into your project, change what you want.

```
curl -O https://github.com/elee1766/tuxcss/releases/latest/download/tux.css
```

minified:

```
curl -O https://github.com/elee1766/tuxcss/releases/latest/download/tux.min.css
```

or link directly (fine for prototyping, vendor for production):

```html
<link rel="stylesheet" href="https://elee1766.github.io/tuxcss/tux.css">
```

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

## license

MIT
