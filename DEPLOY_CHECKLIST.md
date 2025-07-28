# Deployment Checklist for GitHub Pages

## Before Pushing to GitHub

### 1. Update Contact Information
Search and replace in all HTML files:
- `support@miradors.app` → Your actual support email
- `miradors.app` → Your GitHub Pages URL will be: `https://[your-github-username].github.io/miradors/`

### 2. Update App Store Links
In `index.html`, replace the `#` in download links with actual App Store URL when available:
```html
<a href="#" class="download-button">Download on the App Store</a>
```

### 3. Add Screenshots
You need to add these images before going live:
- `screenshot-1.png` through `screenshot-5.png` (actual app screenshots)
- `miradors-preview.png` (1200x630px for social media sharing)

## GitHub Pages Setup Steps

### 1. Initialize Git (if not already done)
```bash
cd /Users/taolu/Desktop/test_app/Miradors/website
git init
git add .
git commit -m "Initial website for Miradors app"
```

### 2. Push to GitHub
```bash
git remote add origin https://github.com/[your-username]/miradors.git
git branch -M main
git push -u origin main
```

### 3. Enable GitHub Pages
1. Go to your repository: `https://github.com/[your-username]/miradors`
2. Click on "Settings" tab
3. Scroll down to "Pages" section
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"

### 4. Access Your Site
Your site will be available at:
```
https://[your-username].github.io/miradors/
```

Note: It may take a few minutes for the site to become available.

## App Store Connect URLs

Once your GitHub Pages site is live, use these URLs in App Store Connect:

- **Support URL**: `https://[your-username].github.io/miradors/support.html`
- **Privacy Policy URL**: `https://[your-username].github.io/miradors/privacy-policy.html`
- **Marketing URL**: `https://[your-username].github.io/miradors/`

## Quick Test Links
After deployment, test all these links work:
- [ ] Homepage loads
- [ ] Privacy Policy accessible
- [ ] Support page accessible
- [ ] All internal links work
- [ ] Email links open email client

## Custom Domain (Optional)
If you want to use a custom domain later:
1. Add a `CNAME` file with your domain
2. Configure DNS settings with your domain provider
3. Enable HTTPS in GitHub Pages settings