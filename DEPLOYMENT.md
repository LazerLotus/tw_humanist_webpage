# Deployment Guide for Taiwanese Humanist Institute Website

## GitHub Pages Setup

### 1. Create GitHub Repository

1. Go to GitHub and create a new repository named `tw_humanist_webpage`
2. Make it public (required for free GitHub Pages)
3. Upload all the files from this project to the repository

### 2. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to "Pages" section
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"

### 3. Custom Domain Setup

#### Update CNAME File

1. Edit the `CNAME` file in your repository
2. Replace the placeholder with your actual domain name (e.g., `taiwanesehumanist.org`)

#### Update HTML Meta Tags

1. Edit `index.html`
2. Replace all instances of `yourdomain.com` with your actual domain
3. Update the sitemap.xml file with your domain
4. Update robots.txt with your domain

#### DNS Configuration

Configure your domain's DNS settings with your domain provider:

**Option A: A Records (Recommended)**

```
A     @     185.199.108.153
A     @     185.199.109.153
A     @     185.199.110.153
A     @     185.199.111.153
```

**Option B: CNAME Record**

```
CNAME  @     yourusername.github.io
```

### 4. SSL Certificate

GitHub Pages automatically provides SSL certificates for custom domains. It may take up to 24 hours to activate.

## File Structure

```
tw_humanist_webpage/
├── index.html          # Main website file
├── styles.css          # CSS styles
├── script.js           # JavaScript functionality
├── 404.html           # Custom 404 page
├── CNAME              # Custom domain configuration
├── sitemap.xml        # SEO sitemap
├── robots.txt         # Search engine crawling rules
├── README.md          # Project documentation
├── .gitignore         # Git ignore rules
└── DEPLOYMENT.md      # This file
```

## Testing Locally

Before deploying, test the website locally:

```bash
# Using Python (if installed)
python -m http.server 8000

# Using Node.js (if installed)
npx serve .

# Using PHP (if installed)
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## Post-Deployment Checklist

- [ ] Website loads correctly at your custom domain
- [ ] All links work properly
- [ ] Contact form is functional (you may need to set up form handling)
- [ ] Mobile responsiveness works
- [ ] SEO meta tags are correct
- [ ] Google Analytics is set up (optional)
- [ ] Social media links are updated
- [ ] Contact information is accurate

## Form Handling

The contact form currently shows a success message but doesn't actually send emails. To make it functional, you can:

1. **Use a form service** like Formspree, Netlify Forms, or Google Forms
2. **Set up a backend** with services like Vercel, Netlify, or Heroku
3. **Use email services** like SendGrid or Mailgun

## Maintenance

- Update content regularly
- Monitor website performance
- Keep dependencies updated
- Backup your repository regularly

## Troubleshooting

### Common Issues:

1. **Domain not working**: Check DNS settings and wait up to 24 hours
2. **SSL certificate issues**: Wait for automatic SSL activation
3. **Images not loading**: Check file paths and ensure images are in the repository
4. **Form not working**: Set up proper form handling service

### Support:

- GitHub Pages documentation: https://docs.github.com/en/pages
- Custom domain setup: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site
