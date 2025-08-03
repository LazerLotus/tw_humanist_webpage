# Assets Directory

This directory contains additional assets for the Taiwanese Humanist Institute website.

## Folder Structure

```
assets/
├── icons/          # Custom icons and favicon
├── fonts/          # Custom fonts (if any)
└── README.md       # This file
```

## Icons Directory

### Favicon

- `favicon.ico` - Main favicon for the website
- `favicon-16x16.png` - 16x16 favicon
- `favicon-32x32.png` - 32x32 favicon
- `apple-touch-icon.png` - Apple touch icon (180x180)

### Custom Icons

- Place custom SVG icons here
- Use descriptive filenames
- Optimize SVG files for web

## Fonts Directory

### Custom Fonts

- Place any custom font files here
- Include multiple formats (woff2, woff, ttf)
- Use descriptive filenames

## Usage Examples

### Favicon in HTML

```html
<link rel="icon" type="image/x-icon" href="assets/icons/favicon.ico" />
<link
  rel="icon"
  type="image/png"
  sizes="32x32"
  href="assets/icons/favicon-32x32.png"
/>
<link
  rel="icon"
  type="image/png"
  sizes="16x16"
  href="assets/icons/favicon-16x16.png"
/>
<link
  rel="apple-touch-icon"
  sizes="180x180"
  href="assets/icons/apple-touch-icon.png"
/>
```

### Custom Fonts in CSS

```css
@font-face {
  font-family: "CustomFont";
  src: url("../assets/fonts/custom-font.woff2") format("woff2"), url("../assets/fonts/custom-font.woff")
      format("woff");
  font-weight: normal;
  font-style: normal;
}
```

## File Guidelines

- Keep file sizes small for fast loading
- Use appropriate formats for each asset type
- Include fallbacks for older browsers
- Test across different devices and browsers
