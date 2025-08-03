# Images Directory

This directory contains all images used in the Taiwanese Humanist Institute website.

## Folder Structure

```
images/
├── hero/           # Hero section images
├── about/          # About section images
├── programs/       # Program-related images
├── team/           # Team member photos
└── logos/          # Organization logos and branding
```

## Image Guidelines

### Recommended Formats

- **WebP** (preferred for best performance)
- **JPEG** (for photographs)
- **PNG** (for logos and graphics with transparency)
- **SVG** (for icons and simple graphics)

### Image Sizes

- **Hero Images**: 1920x1080px or larger
- **About Images**: 800x600px
- **Program Images**: 600x400px
- **Team Photos**: 400x400px (square)
- **Logos**: 200x200px or smaller

### Optimization

- Compress images for web use
- Use descriptive filenames
- Include alt text for accessibility
- Consider lazy loading for better performance

## Usage Examples

### In HTML

```html
<!-- Hero image -->
<img src="images/hero/hero-main.jpg" alt="Taiwanese Humanist Institute" />

<!-- About section image -->
<img src="images/about/team-working.jpg" alt="Team collaboration" />

<!-- Program image -->
<img src="images/programs/disaster-relief.jpg" alt="Disaster relief training" />

<!-- Logo -->
<img src="images/logos/thi-logo.png" alt="THI Logo" />
```

### In CSS

```css
.hero {
  background-image: url("../images/hero/hero-bg.jpg");
}
```

## File Naming Convention

- Use lowercase letters
- Separate words with hyphens
- Include dimensions if multiple sizes exist
- Example: `hero-main-1920x1080.jpg`

## Adding New Images

1. Choose the appropriate folder
2. Optimize the image for web
3. Use descriptive filename
4. Update HTML/CSS to reference the new image
5. Test on different screen sizes
