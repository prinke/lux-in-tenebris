# Lux in Tenebris

Source for **Lux in Tenebris**, a blog by prinke on theology, software and other things,
at [lux.prinke.dev](https://lux.prinke.dev). Built with [Hugo](https://gohugo.io) and
[Scriptorium](https://github.com/prinke/scriptorium), a Dark Academia theme included here
as a git submodule. Comments are handled by [Giscus](https://giscus.app) through this
repository's Discussions.

## Get it

```sh
git clone --recurse-submodules https://github.com/prinke/lux-in-tenebris.git
```

If you already cloned without submodules: `git submodule update --init`.

## Run it

```sh
hugo server -D
```

Requires Hugo 0.158 or newer (the standard edition is enough).

## Layout

| Path | What it holds |
|---|---|
| `content/` | Published posts: `theologia/`, `machina/`, `miscellanea/`, plus About, Search, Catalogue, Index |
| `hugo.toml` | Site settings, section labels and colors, ScriptTagger and Giscus |
| `themes/scriptorium/` | The theme (submodule). Its design rules are in `STYLEGUIDE.md` there |
| `config/development/` | Settings used only by `hugo server` |
| `drafts/` | Not in this repository. Unfinished posts live in a separate private repository cloned here; `hugo server` previews them, production builds ignore them |

## Changing the theme

Theme changes go to the theme's own repository:

```sh
cd themes/scriptorium
# edit, then
git commit -am "…" && git push
cd ../..
git add themes/scriptorium && git commit -m "Update theme"
```

To pull the latest theme: `git submodule update --remote themes/scriptorium`, then commit.
Site-only tweaks can go in `assets/css/custom.css`, `i18n/en.toml` and
`layouts/_partials/hooks/` without touching the theme.

## License

The code in this repository is under the [GNU General Public License v3.0](LICENSE).
