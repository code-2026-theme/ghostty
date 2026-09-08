<p align="center">
  <img src="assets/logo.svg" alt="code-2026" width="96" />
</p>

# code-2026 — Ghostty

Dark and light themes for [Ghostty](https://ghostty.org), ported from VS Code's
**Dark Modern 2026**: red keywords, purple functions, teal types and light-blue strings.

## The code-2026 family

| Target | Repository | |
| --- | --- | --- |
| Neovim | [code-2026-theme/nvim](https://github.com/code-2026-theme/nvim) | colorscheme plugin |
| Ghostty | [code-2026-theme/ghostty](https://github.com/code-2026-theme/ghostty) | **this repo** |
| kitty | [code-2026-theme/kitty](https://github.com/code-2026-theme/kitty) | terminal theme |
| Xcode | [code-2026-theme/xcode](https://github.com/code-2026-theme/xcode) | editor theme |
| Obsidian | [code-2026-theme/obsidian](https://github.com/code-2026-theme/obsidian) | app theme |
| Yazi | [code-2026-theme/yazi](https://github.com/code-2026-theme/yazi) | file manager |

Every port shares one palette, so `:terminal` inside Neovim renders identically to the host
terminal.

## Install

Use the install script (backs up existing themes):

```sh
./install.sh
```

Or copy the theme into Ghostty's themes directory:

```sh
cp themes/code-2026.conf ~/.config/ghostty/themes/code-2026
# or for the light variant:
cp themes/light-2026.conf ~/.config/ghostty/themes/light-2026
```

Then in `~/.config/ghostty/config`:

```conf
theme = code-2026
# or
theme = light-2026
```

Or keep this repo cloned and point at it directly:

```conf
config-file = /path/to/code-2026/themes/code-2026.conf
```

## Palette

| | Normal | | Bright |
| --- | --- | --- | --- |
| black | `#202122` | bright black | `#555555` |
| red | `#ff7b72` | bright red | `#ffa198` |
| green | `#7ee787` | bright green | `#91eb99` |
| yellow | `#cd9731` | bright yellow | `#ffa657` |
| blue | `#79c0ff` | bright blue | `#a5d6ff` |
| magenta | `#d2a8ff` | bright magenta | `#b267e6` |
| cyan | `#4ec9b0` | bright cyan | `#71d4c0` |
| white | `#bbbebf` | bright white | `#ffffff` |

Background `#121314`, foreground `#bbbebf`, cursor `#bbbebf` on `#121314`, selection
`#276782` with `#ffffff` text.

### Light palette

| | Normal | | Bright |
| --- | --- | --- | --- |
| black | `#f0f1f2` | bright black | `#999999` |
| red | `#cf222e` | bright red | `#cf222e` |
| green | `#116329` | bright green | `#116329` |
| yellow | `#953800` | bright yellow | `#953800` |
| blue | `#0550ae` | bright blue | `#0550ae` |
| magenta | `#8250df` | bright magenta | `#8250df` |
| cyan | `#116329` | bright cyan | `#116329` |
| white | `#202020` | bright white | `#ffffff` |

Background `#FFFFFF`, foreground `#202020`, cursor `#0069CC` on `#FFFFFF`, selection
`#C2DAF5` with `#202020` text.

## Credits

Palette from Microsoft's VS Code **Dark Modern 2026** theme, by way of
[D0nw0r/dark2026.nvim](https://github.com/D0nw0r/dark2026.nvim) (MIT).

## License

[MIT](LICENSE)
