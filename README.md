# Docsify Sidebar Expand Collapse

A Docsify v5 plugin that makes top-level sidebar sections collapsible.

## Demos
Docsify Site:  
https://docs.hibbittsdesign.org

Docsify-This Preview:  
https://preview.docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/hibbitts-design-org-docs/master/docs/&homepage=01.overview/overview.md&name=Grav%20CMS%20in%20Open%20Education%20and%20Publishing&searchbox=true&sidebar=true&loadSidebar=true&subMaxLevel=0&sidebar-collapse=true#/

Docsify-This v2 Preview:  
https://preview-v2.docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/hibbitts-design-org-docs/master/docs/&homepage=01.overview/overview.md&name=Grav%20CMS%20in%20Open%20Education%20and%20Publishing&searchbox=true&sidebar=true&loadSidebar=true&subMaxLevel=0&sidebar-collapse=true#

## Features
- Optional accordion behavior - only one section open at a time
- Chevrons matching Docsify v5 design (right-aligned only)
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
- Makes all top-level sidebar sections collapsible with right-aligned chevron indicators
- Expands the section containing the current page
- Closes other sections when you navigate (in accordion mode)

**Note:** This plugin only supports right-aligned chevrons.

## Configuration (Optional)

To allow multiple sections to be open simultaneously:
```html
<script>
  window.$docsify = {
    sidebarExpandCollapse: {
      accordion: false  // Allow multiple sections open at once (default: true)
    }
  }
</script>
```

### Options

| Option | Type | Default | Description |
|--------|------|---------|-------------|
| `accordion` | boolean | `true` | Only allow one section to be open at a time |

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
