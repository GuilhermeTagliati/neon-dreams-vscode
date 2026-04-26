# Neon Dreams

A dark terminal-inspired Visual Studio Code theme built on the visual language of **MONAD Finance (My finance project I've been working on)** .

The overall feeling is a modern command-line interface: near-black green backgrounds, structured borders, muted text hierarchy, and a single neon accent that carries all active states. Think CRT phosphor display, financial terminal, or a quiet cyberpunk control room.

## Design principles

- **Neon green is the only high-brightness accent.** Everything else supports it.
- Backgrounds are layered from deepest (`#030603`) to widget-level (`#121f12`) to create depth without noise.
- Text uses a four-level ink scale — primary, secondary, muted, disabled — all in green-tinted whites, never pure white.
- Semantic colors (error red, warning yellow, info blue) are intentionally distinct from the green palette so they are never confused with structural UI elements.
- Keywords are **bold** — distinction by weight in addition to color.

## Color palette

| Role             | Color     |
| ---------------- | --------- |
| Neon accent      | `#00e87a` |
| Primary text     | `#d8f5d8` |
| Secondary text   | `#9fcf9f` |
| Muted / comments | `#6f936f` |
| Borders          | `#294229` |
| Error            | `#ff4d6d` |
| Warning          | `#ffd166` |
| Info / Types     | `#4f8cff` |

## Syntax highlighting

| Token                        | Color            |
| ---------------------------- | ---------------- |
| Keywords                     | `#00e87a` bold   |
| Functions                    | `#66f2a8`        |
| Classes / Types / Interfaces | `#4f8cff`        |
| Strings                      | `#9fcf9f`        |
| Numbers / Constants          | `#4f8cff`        |
| Comments                     | `#6f936f` italic |
| Properties                   | `#d8f5d8`        |
| Decorators                   | `#ffd166`        |
| Invalid                      | `#ff4d6d`        |

## Terminal

The integrated terminal uses the same palette so it feels native to the theme. ANSI bright white is the only exception — it stays `#ffffff` for compatibility with CLI tools that rely on it.

## Accessibility

The theme is designed to be readable during long coding sessions and usable by people with color vision deficiency:

- Every active state uses at least two visual cues (color + weight, or color + background + border).
- Error, warning, and info colors are clearly distinct from each other and from the neon green.
- Text contrast levels follow a readable hierarchy even in reduced-color conditions.
