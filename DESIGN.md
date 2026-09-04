# Pripyat design notes

## The idea

Pripyat draws visual inspiration from the HBO miniseries *Chernobyl*. It should feel stark, industrial, and weathered without turning the catastrophe into novelty. Near-black green surfaces suggest soot and protective clothing. Concrete haze keeps text readable, oxidized steel separates informational states, and radiation yellow is reserved for focus and warnings.

## Source

Both wallpapers were created by nibra180 using ChatGPT. The primary 6880x2880 wallpaper is dominated by soot green, wet concrete, oxidized blue-green steel, and pale yellow-gray haze. Its quantized dominant colors include `#181E1B`, `#2B3430`, `#3C4844`, `#49554E`, `#69756A`, `#989F8B`, and `#C1C5B1`. The small warm highlight cluster around `#A6A17D` is amplified into radiation yellow for clear focus states.

## Palette

| Role | Color | Use |
| --- | --- | --- |
| Pripyat shadow | `#080C0A` | Deepest surface and scrim |
| Soot green | `#111714` | Main background |
| Wet concrete | `#28342F` | Raised surfaces |
| Contaminated glass | `#34463E` | Selection |
| Dusty sage | `#637268` | Muted text and dividers |
| Concrete haze | `#D7DBC5` | Main text |
| White respirator | `#F2F4E6` | Bright text and cursor |
| Radiation yellow | `#D6D85F` | Focus, warnings, and primary accent |
| Moss | `#94B86B` | Success and positive state |
| Oxidized steel | `#6F9C98` | Information and links |
| Dosimeter cyan | `#83B8AD` | Links and network activity |
| Rust | `#C06F52` | Errors and high temperature |
| Warning amber | `#C79558` | Secondary warning state |
| Filter brass | `#A6A17D` | Special syntax, process data, and ANSI magenta role |

## Rules

1. Keep large surfaces near-black and green. The wallpaper already contains broad middle-gray areas.
2. Reserve radiation yellow for focus, selection, warnings, and short meter segments.
3. Use rust only for errors, destructive states, and high temperatures.
4. Use oxidized steel and cyan for information, links, and network activity.
5. Keep primary text pale and warm so it remains readable against every dark surface.
6. Use filter brass instead of purple for special syntax and secondary process data.
7. Treat the catastrophe and cleanup workers soberly. Avoid novelty radiation symbols or playful copy.

## Background

`backgrounds/pripyat-00-cleanup-workers.jpg` is the primary background. `backgrounds/pripyat-01-city.png` is the secondary background. Both images are stored directly in the theme and numbered so the primary image sorts first.

## Release checklist

- Test horizontal and vertical shell bars.
- Check launcher, menu, notifications, OSD, Polkit, lock screen, and image picker.
- Check all ANSI colors in a terminal test chart.
- Check Rust, PHP, TypeScript, Markdown, JSON, and diff syntax.
- Check btop meters and selected process rows.
- Check Chromium, VS Code, Neovim, Helix, Pi, and Obsidian.
- Confirm the cleanup workers wallpaper is selected by default and the Pripyat wallpaper remains available as the alternate.
- Keep `preview.png` at 1800x1012 and free of local account, process, and hardware data.
- Keep `preview.webp` at 1200x675 and under about 100KB for the omarchy.org/themes listing.
- Keep the wallpaper and preview attribution in `ASSETS.md` current.
- Reinstall from a clean Git URL to test Omarchy's restricted-theme path.
- List the theme with a pull request to [omacom/omarchy-site](https://github.com/omacom/omarchy-site): add `assets/themes/pripyat.webp` and an alphabetical figure in `themes/index.html`.
