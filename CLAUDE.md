# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Vesper Purple is a VS Code theme extension offering dark and light purple-themed color schemes. This is a pure theme extension with no build system or dependencies - JSON theme files are used directly by VS Code.

## Development Commands

```bash
# Test the theme locally (in VS Code)
# Press F5 to launch Extension Development Host, then select theme

# Package for distribution
npm install -g @vscode/vsce
vsce package

# Publish to marketplace
vsce publish
```

## Architecture

### Theme Files
- `themes/vesper-purple-dark-color-theme.json` - Dark theme (base: `vs-dark`)
- `themes/vesper-purple-light-color-theme.json` - Light theme (base: `vs`)

Each theme JSON contains three sections:
1. **colors** - Editor UI colors (sidebar, tabs, panels, status bar, etc.)
2. **semanticTokenColors** - Language Server Protocol token colors with modifiers
3. **tokenColors** - TextMate scope-based syntax highlighting

### Color System

**Dark Theme Layers:**
- Layer 0: `#000000` (editor background)
- Layer 1: `#0a0a0a` (panels, widgets)
- Layer 2: `#1a1a1a` (hover states, inputs)
- Layer 3: `#2a2a2a` (active selections)

**Primary Palette (Tailwind-aligned):**
- Purple accent: `#a855f7` (primary)
- Pink accent: `#f472b6` (secondary)
- Functions: `#c084fc`
- Numbers: `#fbbf24`
- Foreground: `#e4e0d4` (warm white)

### Style Conventions
- **Italic:** Keywords, types, parameters, comments
- **Bold:** Macros, static modifiers
- **Underline:** Readonly properties

## Key Files

- `PRD.md` - Product requirements with color standards and success metrics
- `improvements.md` - Phase 3 roadmap with detailed color specifications for missing UI categories
- `package.json` - Extension manifest (no npm scripts defined)

## Notes

- Extension icon (`images/icon.png`) is referenced but not yet created
- Target WCAG AA contrast compliance for all color choices
- Refer to `improvements.md` for the canonical color hierarchy when adding new colors
