# Docsify Sidebar Expand Collapse

A Docsify v5 plugin that makes top-level sidebar sections collapsible.

## Demo
https://docs.hibbittsdesign.org

## Features
- Optional accordion behavior - only one section open at a time
- Chevrons matching Docsify v5 design
- Fully accessible (keyboard navigation, ARIA support)
- Auto-expands section with active page

## Installation
1. Download `docsify-sidebar-expand-collapse.js`
2. Add to your project's `plugins` folder
3. Include in your index.html (after Docsify):
```html
<script src="./plugins/docsify-sidebar-expand-collapse.js"></script>
```

## Usage
No configuration needed! The plugin automatically:
- Makes all top-level sidebar sections collapsible
- Expands the section containing the current page
- Closes other sections when you navigate (in accordion mode)

## Configuration (Optional)
```html
<script>
  window.$docsify = {
    sidebarExpandCollapse: {
      accordion: true,      // Only one section open at a time (default: true)
      showChevronsRight: true    // Show chevron indicators on right (default: true)
    }
  }
</script>
```

### Options

| Option | Type | Default | Description |
|--------|------|---------|-------------|
| `accordion` | boolean | `true` | Only allow one section to be open at a time |
| `showChevronsRight` | boolean | `true` | Display chevron indicators on right (› when collapsed, ∨ when expanded) |

## Requirements
- Docsify v5

## Accessibility
This plugin is fully accessible:
- Keyboard navigation with Tab, Enter, and Space keys
- Screen reader support with ARIA attributes
- Visible focus indicators

## Known Issues
- **Auto-generated Sidebar content**: When Docsify auto-generates a table of contents from page headers, manually opened sections may require a second click to display after navigation. For best results, explicitly define all sidebar sections in your `_sidebar.md` file.

## Credits
Original concept by [@Wsine](https://github.com/Wsine)  
Enhanced with assistance from Anthropic Claude AI
