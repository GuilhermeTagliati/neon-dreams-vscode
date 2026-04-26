# Change Log

All notable changes to the "neon-dreams" extension will be documented in this file.

## [0.0.1] — 2026-04-26 — Dark Terminal Green

First public release of **Neon Dreams**, a VS Code theme inspired by the visual identity of MONAD Finance.

Built for developers who spend long hours in the editor and want a focused, readable environment — dark green backgrounds, a single neon accent, and just enough color to communicate meaning without noise.

## [Unreleased]

### Added

- Initial theme definition based on the Neon Dreams spec
- Full UI color coverage: editor, sidebar, activity bar, tabs, status bar, terminal, command palette, inputs, menus, scrollbar, minimap, and git decorations
- TextMate token colors for comments, keywords, strings, numbers, functions, classes, types, properties, decorators, and invalid syntax
- Semantic token colors for all major language constructs
- ANSI terminal color palette aligned with the theme identity

### Changed (Accessibility pass)

- Replaced base palette with higher-contrast variants: backgrounds slightly adjusted, borders more visible (`#294229`)
- Ink text scale clarified: primary text `#d8f5d8`, secondary `#9fcf9f`, muted `#6f936f`, disabled `#3d5c3d`
- Info/type color shifted from `#38bdf8` (cyan) to `#4f8cff` (blue) for better separation from the neon green accent
- Warning color shifted from `#f59e0b` (amber) to `#ffd166` (bright yellow) for stronger contrast on dark backgrounds
- Danger color adjusted from `#ff3a5c` to `#ff4d6d` for slightly better readability
- Keywords (`function`, `const`, `return`, etc.) now render **bold** to distinguish them from identifiers by weight, not just color
- Removed `meta.function-call` from the function token rule — constructor calls like `new ArrayInput()` now resolve to the class color (`#4f8cff`) instead of the function color (`#66f2a8`)
- Removed broad `source` and `meta` scopes from the default variable rule to prevent unintended color overrides
