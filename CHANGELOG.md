# Changelog

All notable changes to the Vesper Purple Ox extension will be documented in this file.

## [0.3.0] - 2025-11-25

### Added
- **Light theme comprehensive enhancement** - now matches dark theme parity:
  - 715 color properties (up from 247)
  - Complete semantic token system with all 19 types + 13 modifiers
  - Language-specific rules for Python, TypeScript, Rust, Go
  - 60+ token color rules for JSX/TSX, CSS/SCSS, JSON/YAML, Shell
  - 88 Monaco editor rules for web compatibility
  - Symbol icons and chart colors
- **Comprehensive UI color support** for both themes:
  - Chat/AI colors (Copilot, Inline Chat)
  - Testing colors (icons, coverage, messages)
  - Debug colors (toolbar, console, icons, expressions)
  - Notebook colors (cells, borders, status)
  - Welcome Page colors
  - Ports, Comments View, Banner colors
  - Command Center and Keybinding colors
- **Complete semantic token system** with all 19 standard types:
  - namespace, class, enum, interface, struct, typeParameter, type
  - parameter, variable, property, enumMember, decorator, event
  - function, method, macro, label, comment, string, keyword, number, regexp, operator
- **13 semantic token modifiers**:
  - readonly (underline), static (bold), deprecated (strikethrough)
  - abstract, async (cyan), documentation, defaultLibrary
- **Language-specific semantic rules** for Python, TypeScript, Rust, Go
- **Enhanced token color rules** (60+ rules) for:
  - JSX/TSX components
  - CSS/SCSS selectors and properties
  - JSON/YAML keys
  - Shell variables
  - Decorators and async/await
- **Symbol icons** with consistent color mapping
- **Chart colors** for data visualization
- **Monaco editor rules** for web compatibility
- **Extension icon** (256x256 PNG)
- **CHANGELOG.md** and updated **README.md**

### Fixed
- Light theme deprecated property warnings
- Light theme using correct `base: "vs"` structure

## [0.2.0] - 2024

### Added
- **Visual enhancements** to dark theme:
  - Pure black background (`#000000`) for maximum contrast
  - More vibrant purple accents (`#a855f7` primary, `#c084fc` functions)
  - Enhanced pink tones (`#f472b6` for variables/properties)
  - Italic styles for semantic tokens (comments, keywords, types, etc.)
- Improved terminal colors using Tailwind CSS palette
- Monaco editor `rules` array for web compatibility

### Fixed
- Deprecated `editorIndentGuide.background` → `editorIndentGuide.background1`
- Selection backgrounds made transparent
- Removed unsupported token background colors
- Invalid fontStyle values corrected

### Changed
- Theme structure from `"type": "dark"` to `"base": "vs-dark"`
- Updated color palette to be more vibrant

## [0.1.0] - 2024

### Added
- Initial release
- Dark theme variant (Vesper Purple Dark)
- Light theme variant (Vesper Purple Light)
- Basic semantic highlighting support
- Git decoration colors
- Bracket pair colorization (6 levels)
- Terminal ANSI colors

---

Based on the [Vesper Purple Theme](https://github.com/xinyao27/vscode-theme) by xinyao27.
