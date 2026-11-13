# prinke.dev

Source for **Lux in Tenebris**, a blog by prinke on theology, software and other things,
at [prinke.dev](https://prinke.dev). Built with [Hugo](https://gohugo.io) and a custom
Dark Academia theme, `DarkAcademia`, in `themes/`.

## Run it

```sh
hugo server
```

Requires Hugo 0.146 or newer (the standard edition is enough).

## Layout

| Path | What it holds |
|---|---|
| `content/` | Published posts: `theologia/`, `machina/`, `miscellanea/`, plus About, Search, Catalogue, Index |
| `themes/DarkAcademia/` | The theme: layouts, CSS, self-hosted fonts, shortcodes. Its design rules are in [`STYLEGUIDE.md`](themes/DarkAcademia/STYLEGUIDE.md) |
| `config/development/` | Settings used only by `hugo server` |
| `drafts/` | Not in this repository. Unfinished posts live in a separate private repository cloned here; `hugo server` previews them, production builds ignore them |

## Writing features

Scripture quotations with verse numbers, margin notes, Greek and Hebrew text,
Latin-labelled callouts (`> [!NB]`, `> [!CAVEAT]`, `> [!ERGO]`), captioned image plates,
code blocks with filenames, and Blue Letter Bible verse pop-ups. See the theme's
style guide for the syntax.

## Fonts

EB Garamond, Cormorant Garamond, UnifrakturMaguntia, JetBrains Mono and Frank Ruhl Libre,
all under the SIL Open Font License. See
[`themes/DarkAcademia/static/fonts/OFL.txt`](themes/DarkAcademia/static/fonts/OFL.txt).
