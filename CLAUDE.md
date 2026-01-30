# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains multiple NeoMutt color schemes. NeoMutt is a command-line email client.

## File Structure

Each color scheme lives in its own subdirectory:

- `yaru/` - Ubuntu Yaru-inspired color scheme (eggplant/aubergine tones)
  - `mutt-colors-ubuntu-yaru-256.neomuttrc` - 256-color mode with hex backgrounds
  - `mutt-colors-ubuntu-yaru-truecolor.neomuttrc` - True color (24-bit) hex values throughout
- `duotone/` - Duotone color scheme (teal/turquoise with bright field green)
  - `duotone.neomuttrc` - True color (24-bit) duotone theme based on Base2Tone Field Dark

## Ubuntu-Yaru Color Palette

| Color Name      | Hex Value | 256-color Approx |
|-----------------|-----------|------------------|
| bg (eggplant)   | #2C001E   | -                |
| bg_alt          | #3B1028   | -                |
| fg              | #F6F5F4   | color255         |
| fg_dim          | #D5CFCA   | color251         |
| comment         | #B7A7B4   | color249         |
| orange          | #E95420   | color202         |
| aubergine       | #772953   | color89          |
| aubergine_dark  | #5E2750   | -                |
| gold            | #F99B15   | color214         |
| green           | #26A269   | color35          |
| teal            | #19B6EE   | color39          |
| red             | #C7162B   | color160         |
| border          | #4A1D33   | color89          |
| selection       | #3D1E2F   | -                |

## NeoMutt Color Scheme Syntax

```
color <object> <foreground> <background> [<pattern>]
```

Key objects styled: `normal`, `error`, `status`, `indicator`, `tree`, `sidebar_*`, `index`, `header`, `hdrdefault`, `quoted`, `quoted1-4`, `body`, `compose`.

## Testing

Source in neomuttrc:
```
source /path/to/yaru/mutt-colors-ubuntu-yaru-256.neomuttrc
```

For true color version, first enable direct color:
```
set color_directcolor = yes
source /path/to/yaru/mutt-colors-ubuntu-yaru-truecolor.neomuttrc
```

Or run directly:
```
neomutt -F /path/to/yaru/mutt-colors-ubuntu-yaru-256.neomuttrc
```
