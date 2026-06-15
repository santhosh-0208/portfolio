# GitHub Pages Portfolio Setup Guide

Your portfolio is now ready to deploy to GitHub Pages! The `static.yml` workflow file is already configured to deploy your HTML files.

## Quick Start

### 1. Push to GitHub
If you haven't already set up the GitHub repository:

```bash
git add .
git commit -m "Convert portfolio to HTML with GitHub Pages setup"
git push origin main
```

### 2. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under "Source", select:
   - **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ (root)**
4. Click **Save**

### 3. GitHub Actions Deployment

The `static.yml` workflow will automatically:
- Trigger on push to the `main` branch
- Build and deploy your portfolio to GitHub Pages
- Make it available at: `https://yourusername.github.io/portfolio` (or your custom domain)

## What's Included

✅ **index.html** - Main portfolio landing page
✅ **styles.css** - Professional dark theme styling
✅ **Project Pages** - Individual HTML pages for each project:
  - `projects/suspension-optimization.html`
  - `projects/self-balancing-robot.html`
  - `projects/adaptive-assembly.html`
✅ **Responsive Design** - Works on mobile, tablet, and desktop
✅ **GitHub Actions Workflow** - Automatic deployment

## Local Testing

To test locally before pushing:

```bash
# Option 1: Use Python's built-in server
python -m http.server 8000

# Option 2: Use Node's http-server
npx http-server

# Then open: http://localhost:8000
```

## Customization

### Update Navigation Links

Edit `index.html` and project HTML files to update:
- Social media links in footer
- Contact information
- Any other personal details

```html
<!-- In footer or navbar -->
<a href="https://github.com/yourusername" target="_blank">GitHub</a>
<a href="https://linkedin.com/in/yourprofile" target="_blank">LinkedIn</a>
```

### Add Images

Place project images in an `images/` folder:
```
portfolio/
├── images/
│   ├── suspension_model.png
│   └── ga_results.png
```

The HTML already references these paths correctly.

### Update Resume Link

Replace `resume.pdf` with your actual resume file in the root directory.

### Change Colors

Edit CSS variables in `styles.css`:

```css
:root {
    --primary-color: #0066cc;
    --secondary-color: #00a3e0;
    --dark-bg: #0a0e27;
    --accent: #00d4ff;
    /* ... customize as needed */
}
```

## Project Structure

```
portfolio/
├── index.html                          # Main portfolio page
├── styles.css                          # All styling
├── resume.pdf                          # Your resume
├── projects/
│   ├── suspension-optimization.html
│   ├── self-balancing-robot.html
│   └── adaptive-assembly.html
├── images/                             # Project images
│   ├── suspension_model.png
│   └── ga_results.png
├── README.md                           # Original markdown (optional)
└── .github/
    └── workflows/
        └── static.yml                  # GitHub Actions workflow
```

## Deployment Status

After pushing, check deployment status:

1. Go to your GitHub repository
2. Click **Actions** tab
3. View the "Deploy static content to Pages" workflow
4. Once it shows ✅, your site is live!

## Custom Domain (Optional)

To use a custom domain:

1. Update DNS settings at your domain registrar
2. In repository Settings → Pages → Custom domain
3. Enter your domain and save

## Troubleshooting

### Pages not deploying
- Ensure `main` branch is selected in Pages settings
- Check Actions tab for workflow errors
- Verify workflow file path: `.github/workflows/static.yml`

### Images not loading
- Check image file paths match HTML references
- Ensure images are committed to git
- Use relative paths: `./images/filename.png`

### Styling not applied
- Hard refresh browser: `Ctrl+Shift+R` or `Cmd+Shift+R`
- Clear browser cache
- Check CSS file is served (check network tab in DevTools)

## Next Steps

1. ✅ Create HTML portfolio
2. ✅ Set up GitHub Actions workflow
3. → Push to GitHub
4. → Enable GitHub Pages in settings
5. → Access your live portfolio!

For more info: https://docs.github.com/en/pages
