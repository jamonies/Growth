# Phantom Template - AI Agent Instructions

## Project Overview
Phantom is a responsive HTML5/CSS3 site template built around a grid of large, colorful, semi-interactive image tiles. The template features a clean, modern design with smooth animations and a mobile-first approach.

## Architecture

### Key Components
- **Template Structure**
  - `index.html`: Main landing page with tile grid layout
  - `generic.html`: Generic content page template
  - `elements.html`: Style guide and UI components
  
### Asset Organization
```
assets/
├── css/          # Compiled CSS files
├── sass/         # Source SCSS files
│   ├── base/     # Core styles
│   ├── components/# Reusable UI components
│   ├── layout/   # Layout structures
│   └── libs/     # Mixins and utilities
└── js/          # JavaScript functionality
```

## Key Patterns and Conventions

### Styling
- SCSS architecture uses the 7-1 pattern (base, components, layout, libs)
- Breakpoint handling uses the `breakpoints` mixin defined in `_breakpoints.scss`
- Responsive grid uses the `html-grid` system from `_html-grid.scss`

### JavaScript Patterns
- jQuery-based functionality in `main.js`
- Mobile detection via `browser.mobile`
- Menu toggle system using `_lock()`, `_show()`, `_hide()`, and `_toggle()`
- Form handling includes auto-resizing textareas and mobile-specific adjustments

### Common Tasks

#### Adding New Tiles
1. Copy an existing `article` element in `index.html`
2. Update classes (style1-6 for color variations)
3. Replace image and content
```html
<article class="style1">
  <span class="image">
    <img src="images/pic01.jpg" alt="" />
  </span>
  <a href="generic.html">
    <h2>Title</h2>
    <div class="content">
      <p>Description</p>
    </div>
  </a>
</article>
```

#### Style Customization
- Color schemes defined in `_vars.scss`
- Tile styles in `_tiles.scss`
- Layout measurements in `_vars.scss` and respective component files

## Dependencies
- jQuery for DOM manipulation and events
- Font Awesome for icons
- Google Fonts (Source Sans Pro)