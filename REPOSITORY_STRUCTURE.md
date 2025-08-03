# Repository Structure

This document outlines the organized structure of the Taiwanese Humanist Institute website repository.

## 📁 Root Directory

```
tw_humanist_webpage/
├── index.html              # Main website file
├── 404.html               # Custom 404 error page
├── CNAME                  # Custom domain configuration
├── robots.txt             # Search engine crawling rules
├── sitemap.xml           # SEO sitemap
├── README.md             # Project documentation
├── DEPLOYMENT.md         # Deployment guide
├── WEBSITE_FEATURES.md   # Features documentation
├── REPOSITORY_STRUCTURE.md # This file
├── package.json          # Project metadata
├── .gitignore           # Git ignore rules
├── css/                 # Stylesheets
├── js/                  # JavaScript files
├── images/              # Image assets
└── assets/              # Additional assets
```

## 📂 CSS Directory

```
css/
└── styles.css           # Main stylesheet
```

## 📂 JavaScript Directory

```
js/
└── script.js            # Main JavaScript file
```

## 📂 Images Directory

```
images/
├── README.md            # Image usage guidelines
├── hero/                # Hero section images
│   └── .gitkeep
├── about/               # About section images
│   └── .gitkeep
├── programs/            # Program-related images
│   └── .gitkeep
├── team/                # Team member photos
│   └── .gitkeep
└── logos/               # Organization logos
    └── .gitkeep
```

### Image Guidelines

- **Hero Images**: 1920x1080px or larger
- **About Images**: 800x600px
- **Program Images**: 600x400px
- **Team Photos**: 400x400px (square)
- **Logos**: 200x200px or smaller

## 📂 Assets Directory

```
assets/
├── README.md            # Assets usage guidelines
├── icons/               # Custom icons and favicon
│   └── .gitkeep
└── fonts/               # Custom fonts (if any)
    └── .gitkeep
```

## 🖼️ Adding Images

### Step 1: Choose the Right Folder

- **Hero images** → `images/hero/`
- **About section images** → `images/about/`
- **Program images** → `images/programs/`
- **Team photos** → `images/team/`
- **Logos** → `images/logos/`

### Step 2: Optimize Your Images

- Use WebP format when possible
- Compress images for web
- Use descriptive filenames
- Include appropriate dimensions

### Step 3: Update HTML/CSS

```html
<!-- Example: Adding a hero image -->
<img src="images/hero/hero-main.jpg" alt="Taiwanese Humanist Institute" />
```

```css
/* Example: Using image as background */
.hero {
  background-image: url("../images/hero/hero-bg.jpg");
}
```

## 📝 File Naming Convention

### Images

- Use lowercase letters
- Separate words with hyphens
- Include dimensions if multiple sizes exist
- Examples:
  - `hero-main-1920x1080.jpg`
  - `team-member-john-doe.jpg`
  - `disaster-relief-training.jpg`
  - `thi-logo.png`

### Assets

- Use descriptive names
- Include file type in name
- Examples:
  - `favicon.ico`
  - `apple-touch-icon.png`
  - `custom-font.woff2`

## 🚀 Deployment Considerations

### GitHub Pages

- All files are properly organized for GitHub Pages
- CSS and JS files are in their respective folders
- Images are organized by purpose
- Assets are separated for easy management

### Performance

- Images are organized for easy optimization
- CSS and JS are in separate folders for caching
- Structure supports lazy loading implementation

## 🔧 Maintenance

### Adding New Content

1. Place images in appropriate folders
2. Update HTML to reference new images
3. Test on different screen sizes
4. Optimize for performance

### Updating Existing Content

1. Replace images with same filename
2. Update alt text if needed
3. Test functionality
4. Commit changes

## 📊 SEO Benefits

### Organized Structure

- Clear separation of content types
- Easy to implement structured data
- Optimized for search engine crawling
- Proper file organization for CDN

### Image Optimization

- Organized for easy compression
- Clear naming for alt text
- Proper folder structure for lazy loading
- Ready for WebP implementation

This structure provides a clean, organized foundation for the Taiwanese Humanist Institute website that's easy to maintain and scale.
