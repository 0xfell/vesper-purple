# Purple Vesper Theme - Product Requirements Document

## Overview

Purple Vesper Theme is a Visual Studio Code color theme extension that provides a dark purple aesthetic for developers who prefer a purple-accented coding environment. This project is based on the [Vesper Purple Theme](https://github.com/xinyao27/vscode-theme) by xinyao27.

## Goals

### Primary Goals
1. **Replicate** the Vesper Purple Theme with high fidelity
2. **Provide** both dark and light theme variants
3. **Ensure** readability and visual comfort for extended coding sessions
4. **Maintain** semantic highlighting support for modern language features

### Secondary Goals
1. Create a foundation for future visual improvements and customizations
2. Publish to VS Code Marketplace for easy installation

## Theme Variants

### Purple Vesper Dark
- **Base**: `vs-dark`
- **Primary Background**: `#0a0a0a` (near black)
- **Primary Foreground**: `#dbd7caee` (warm white)
- **Accent Color**: `#c391e6` (light purple)
- **Secondary Accent**: `#ed9cc2` (pink)

### Purple Vesper Light
- **Base**: `vs`
- **Primary Background**: `#f5f5f5` (light gray)
- **Primary Foreground**: `#323232` (dark gray)
- **Accent Color**: `#9066df` (purple)
- **Secondary Accent**: `#ec4899` (pink)

## Color Palette

### Core Colors (Dark Theme)

| Element | Color | Hex Code |
|---------|-------|----------|
| Background | Near Black | `#0a0a0a` |
| Surface | Dark Gray | `#222222` |
| Foreground | Warm White | `#dbd7caee` |
| Primary Purple | Light Purple | `#c391e6` |
| Secondary Pink | Soft Pink | `#ed9cc2` |
| Comments | Faded White | `#ffffff4f` |
| Strings | Gray | `#a3a3a3` |
| Numbers/Booleans | Yellow | `#eab308` |
| Errors | Red | `#fca5a5` |
| Warnings | Amber | `#f59e0b` |
| Info | Blue | `#0369a1` |
| Success | Green | `#16a34a` |

### Syntax Highlighting

| Token Type | Dark Theme | Light Theme |
|------------|------------|-------------|
| Functions | `#c391e6` | `#9066df` |
| Variables | `#ed9cc2` | `#ec4899` |
| Constants | `#ed9cc2` | `#ed9cc2` |
| Keywords | `#ffffff9f` | `#ed9cc2` |
| Strings | `#a3a3a3` | `#525252` |
| Comments | `#ffffff4f` | `#737373` |
| Numbers | `#eab308` | `#eab308` |
| Types | `#ed9cc2` | `#ed9cc2` |
| Tags (HTML) | `#c391e6` | `#9066df` |
| Attributes | `#ed9cc2` | `#ec4899` |

## Technical Specifications

### Requirements
- VS Code version: `^1.64.0`
- Extension category: Themes

### File Structure
```
purple-vesper-vscode/
├── themes/
│   ├── purple-vesper-dark-color-theme.json
│   └── purple-vesper-light-color-theme.json
├── images/
│   └── icon.png (to be added)
├── package.json
├── README.md
├── LICENSE
├── .gitignore
├── .vscodeignore
└── PRD.md
```

### Features
- [x] Dark theme variant
- [x] Light theme variant
- [x] Semantic highlighting support
- [x] Full UI color customization
- [x] Terminal color support
- [x] Git decoration colors
- [x] Bracket pair colorization
- [x] Diff editor colors

## Installation & Testing

### Local Development
1. Open the project folder in VS Code
2. Press `F5` to launch Extension Development Host
3. In the new window, go to `File > Preferences > Color Theme`
4. Select "Purple Vesper Dark" or "Purple Vesper Light"

### Packaging
```bash
npm install -g @vscode/vsce
vsce package
```

### Publishing
```bash
vsce publish
```

## Future Improvements (Phase 2)

### Visual Enhancements
- [ ] Fine-tune contrast ratios for better accessibility
- [ ] Adjust syntax highlighting colors based on user feedback
- [ ] Add italic styles for certain token types
- [ ] Improve diff editor color visibility
- [ ] Enhance minimap colors

### Additional Variants
- [ ] Purple Vesper Dark High Contrast
- [ ] Purple Vesper Dark Soft (reduced contrast)

### Quality Improvements
- [ ] Add screenshot to README
- [ ] Create icon.png for extension
- [ ] Add CHANGELOG.md
- [ ] Set up automated testing for color consistency

## Success Metrics

1. **Readability**: All text elements have sufficient contrast ratio (WCAG AA compliance)
2. **Consistency**: Colors are consistent across all supported languages
3. **Completeness**: All UI elements have defined colors (no fallback to defaults)
4. **User Satisfaction**: Positive feedback from initial users

## References

- Original Theme: https://github.com/xinyao27/vscode-theme
- VS Code Theme Documentation: https://code.visualstudio.com/api/references/theme-color
- TextMate Scope Reference: https://macromates.com/manual/en/language_grammars

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 0.1.0 | 2024 | Initial release - Replicated Vesper Purple Theme |

---

*This PRD is a living document and will be updated as the project evolves.*
