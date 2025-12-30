# Docsify Sidebar Collapse

A Docsify v5 plugin that makes top-level sidebar sections collapsible with accordion behavior.

## Demo
https://docs.hibbittsdesign.org

## Features

- Accordion behavior - only one section open at a time
- Chevrons matching Docsify v5 design
- Fully accessible (keyboard navigation, ARIA support)
- Smooth hover effects
- Auto-expands section with active page

## Installation

1. Download `docsify-sidebar-collapse.js`
2. Add to your project's `plugins` folder
3. Include in your index.html (after Docsify):
```html
<script src="./plugins/docsify-sidebar-collapse.js"></script>
```

## Usage

No configuration needed! The plugin automatically:
- Makes all top-level sidebar sections collapsible
- Expands the section containing the current page
- Closes other sections when you navigate

## Configuration (Optional)

To hide chevron indicators:
```html

  window.$docsify = {
    sidebarCollapse: {
      showChevrons: false
    }
  }

```

## Requirements

- Docsify v5

## Accessibility

This plugin is fully accessible:
- Keyboard navigation with Tab, Enter, and Space keys
- Screen reader support with ARIA attributes
- Visible focus indicators

## Credits

Original concept by [@Wsine](https://github.com/Wsine)  
Enhanced with assistance from Anthropic Claude AI
