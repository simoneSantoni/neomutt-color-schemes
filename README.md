# NeoMutt Color Schemes

A collection of color schemes for [NeoMutt](https://neomutt.org/), a command-line email client.

## Color Schemes

### Yaru (`yaru/`)

Inspired by the [Ubuntu Yaru](https://github.com/ubuntu/yaru) color palette, featuring the iconic eggplant/aubergine tones.

- Full styling for all NeoMutt UI elements (index, sidebar, headers, compose view)
- Distinct colors for message states (new, read, flagged, deleted)
- Quoted text levels with different colors
- URL and email address highlighting
- GPG/PGP signature status coloring
- Two versions available:
  - **256-color** - Works in most terminals
  - **True color** - Uses exact hex values for terminals with 24-bit color support

#### Color Palette

| Color           | Hex       | Usage                          |
|-----------------|-----------|--------------------------------|
| Eggplant (bg)   | `#2C001E` | Background                     |
| Aubergine       | `#772953` | Accents, replied messages      |
| Orange          | `#E95420` | Ubuntu orange, links, indicator|
| Gold            | `#F99B15` | Dates, warnings                |
| Green           | `#26A269` | Messages to me, good signature |
| Teal            | `#19B6EE` | New/unread messages, subjects  |
| Red             | `#C7162B` | Flagged, deleted, errors       |
| Foreground      | `#F6F5F4` | Normal text                    |

#### Installation

**256-color version** - add to your `neomuttrc`:

```neomuttrc
source /path/to/yaru/mutt-colors-ubuntu-yaru-256.neomuttrc
```

**True color version** - requires a terminal with 24-bit color support:

```neomuttrc
set color_directcolor = yes
source /path/to/yaru/mutt-colors-ubuntu-yaru-truecolor.neomuttrc
```

### Duotone (`duotone/`)

A duotone theme featuring teal/turquoise with bright field green, based on [Base2Tone Field Dark](https://github.com/atelierbram/Base2Tone-kitty) by Bram de Haan.

- True color only (requires 24-bit color support)
- Teal-gray dark background with green/cyan accent tones
- Full styling for all NeoMutt UI elements

#### Color Palette

| Color           | Hex       | Usage                          |
|-----------------|-----------|--------------------------------|
| Dark teal-gray  | `#18201e` | Background                     |
| Teal            | `#0fbda0` | Primary accent, URLs, indicator|
| Bright teal     | `#25d0b4` | Messages to me                 |
| Cyan            | `#40ddc3` | Old messages, quoted text      |
| Bright cyan     | `#88f2e0` | New/unread messages, subjects  |
| Green           | `#3be381` | Tree, good signatures          |
| Bright green    | `#55ec94` | Flagged messages, errors       |
| Mint            | `#85ffb8` | Expired, search highlight      |
| Foreground      | `#8ea4a0` | Normal text                    |

#### Installation

Requires a terminal with 24-bit color support. Add to your `neomuttrc`:

```neomuttrc
set color_directcolor = yes
source /path/to/duotone/duotone.neomuttrc
```

## Testing

Test a color scheme without modifying your config:

```bash
neomutt -F /path/to/yaru/mutt-colors-ubuntu-yaru-256.neomuttrc
```

## Credits

- Yaru scheme based on [yaru.nvim](https://github.com/simoneSantoni/yaru.nvim) by Simone Santoni.
- Duotone scheme based on [Base2Tone-kitty](https://github.com/atelierbram/Base2Tone-kitty) by Bram de Haan.

## License

MIT
