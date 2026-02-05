# Deployment Guide - Vietnam Market Study

Complete guide to deploying your Vietnam Market Study documentation site.

## 📋 Pre-Deployment Checklist

Before deploying, ensure you have:

- [ ] All content files reviewed
- [ ] Tables and data verified
- [ ] Code examples tested
- [ ] Links checked (no broken links)
- [ ] Images optimized (if any)
- [ ] Site name customized in `index.html`
- [ ] Repository URL updated in `index.html`

## 🚀 Deployment Options

### Option 1: GitHub Pages (Recommended)

**Advantages**:
- Free hosting
- Custom domain support
- Automatic HTTPS
- Easy updates (just push changes)

#### Step-by-Step GitHub Pages Deployment

**1. Create GitHub Repository**

```bash
# Navigate to your documentation folder
cd vietnam-market-docs

# Initialize Git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Vietnam Market Study documentation"
```

**2. Create Repository on GitHub**

- Go to https://github.com/CHAN084ntu
- Click "New repository"
- Name it: `vietnam-market-study` (or your preferred name)
- Description: "Comprehensive quantitative analysis of Vietnam stock market"
- Public or Private (your choice)
- Don't initialize with README (you already have one)
- Click "Create repository"

**3. Push to GitHub**

```bash
# Add remote
git remote add origin https://github.com/CHAN084ntu/vietnam-market-study.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**4. Enable GitHub Pages**

- Go to your repository on GitHub
- Click **Settings** (⚙️)
- Scroll to **Pages** in the left sidebar
- Under **Source**:
  - Branch: `main`
  - Folder: `/ (root)`
- Click **Save**

**5. Access Your Site**

After 2-5 minutes, your site will be live at:
```
https://CHAN084ntu.github.io/vietnam-market-study/
```

### Option 2: Custom Domain (Optional)

If you want to use your own domain:

**1. Create CNAME File**

```bash
echo "docs.yourdomain.com" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```

**2. Configure DNS**

Add a CNAME record in your DNS settings:
```
Type: CNAME
Name: docs (or your subdomain)
Value: CHAN084ntu.github.io
```

**3. Enable in GitHub**

- Settings > Pages
- Custom domain: `docs.yourdomain.com`
- Save
- Wait for DNS propagation (5-60 minutes)

### Option 3: Netlify

**Advantages**:
- Drag-and-drop deployment
- Instant preview URLs
- Built-in form handling

**Steps**:

1. Go to [netlify.com](https://netlify.com)
2. Sign up / Log in
3. Click "Add new site" > "Deploy manually"
4. Drag the `vietnam-market-docs` folder
5. Site deployed instantly!

**Alternative**: Connect to GitHub for automatic deploys

### Option 4: Vercel

**Advantages**:
- Fast global CDN
- Automatic HTTPS
- Serverless functions (if needed)

**Steps**:

1. Go to [vercel.com](https://vercel.com)
2. Sign up with GitHub
3. Click "New Project"
4. Import `vietnam-market-study` repository
5. Framework: Select "Other"
6. Deploy

### Option 5: Self-Hosting

Host on your own server:

**Apache**:
```apache
<VirtualHost *:80>
    ServerName vietnam-study.yourdomain.com
    DocumentRoot /var/www/vietnam-market-docs
    
    <Directory /var/www/vietnam-market-docs>
        Options Indexes FollowSymLinks
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>
```

**Nginx**:
```nginx
server {
    listen 80;
    server_name vietnam-study.yourdomain.com;
    root /var/www/vietnam-market-docs;
    index index.html;
    
    location / {
        try_files $uri $uri/ /index.html;
    }
}
```

## 🔧 Post-Deployment Tasks

### 1. Update Repository URL

Edit `index.html` - find this section:

```javascript
window.$docsify = {
  // ...
  repo: 'https://github.com/CHAN084ntu/vietnam-market-study',
  // ...
};
```

Change to your actual repository URL.

### 2. Test All Links

Visit your deployed site and:
- [ ] Click through all navigation links
- [ ] Test search functionality
- [ ] Verify code blocks display correctly
- [ ] Check tables render properly
- [ ] Test on mobile device

### 3. Enable Analytics (Optional)

Add Google Analytics to `index.html`:

```html
<script>
  window.$docsify = {
    ga: 'G-XXXXXXXXXX',  // Your GA4 measurement ID
    // ... other config
  };
</script>
<script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/ga.min.js"></script>
```

### 4. Add Social Meta Tags

For better sharing on social media, add to `<head>` in `index.html`:

```html
<!-- Open Graph -->
<meta property="og:title" content="Vietnam Market Study">
<meta property="og:description" content="Comprehensive quantitative analysis of Vietnam stock market">
<meta property="og:type" content="website">
<meta property="og:url" content="https://CHAN084ntu.github.io/vietnam-market-study/">

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Vietnam Market Study">
<meta name="twitter:description" content="Quantitative analysis and trading guide for Vietnam equities">
```

## 🔄 Updating Your Site

After initial deployment, to update content:

```bash
# Edit your markdown files
# ... make changes ...

# Commit and push
git add .
git commit -m "Update: Added Q4 2024 data"
git push

# GitHub Pages will automatically rebuild (2-5 minutes)
```

## 🐛 Troubleshooting

### Site Shows 404 Error

**Problem**: Page not found after enabling GitHub Pages

**Solutions**:
1. Wait 5-10 minutes (initial deployment can be slow)
2. Check branch is set to `main` in Pages settings
3. Verify folder is set to `/ (root)`
4. Ensure `index.html` exists in root directory

### Styles Not Loading

**Problem**: Site looks unstyled

**Solutions**:
1. Check browser console for errors (F12)
2. Verify CDN links in `index.html` are accessible
3. Clear browser cache (Ctrl+Shift+R / Cmd+Shift+R)
4. Check if ad blocker is interfering

### Navigation Not Working

**Problem**: Clicking links doesn't change pages

**Solutions**:
1. Verify all `.md` files exist in correct directories
2. Check `_sidebar.md` paths match actual file locations
3. Ensure file names are exactly as referenced (case-sensitive)
4. Check browser console for JavaScript errors

### Search Not Working

**Problem**: Search box doesn't find content

**Solutions**:
1. Wait for initial indexing (can take a minute on first load)
2. Search plugin loaded? Check `index.html`
3. Try refreshing the page
4. Check browser console for errors

### Images Not Displaying

**Problem**: Images show as broken

**Solutions**:
1. Verify image files are committed to Git
2. Check image paths in markdown (relative paths)
3. Ensure images are in web format (PNG, JPG, SVG)
4. Check file size (keep under 500KB)

## 🎯 Best Practices

### Content Organization

1. **One topic per file** - Don't create mega-files
2. **Consistent naming** - Use kebab-case (`file-name.md`)
3. **Logical hierarchy** - Nest content appropriately
4. **Cross-linking** - Link related sections

### Performance

1. **Optimize images** - Compress before uploading
2. **Lazy loading** - Docsify does this automatically
3. **Minimize dependencies** - Only load needed plugins
4. **CDN assets** - Use CDN links (already configured)

### Maintenance

1. **Regular updates** - Keep data current
2. **Version control** - Use meaningful commit messages
3. **Backup** - GitHub is your backup
4. **Changelog** - Document major changes

## 📊 Monitoring

### GitHub Pages Stats

View deployment status:
- Repository > Environments > github-pages

### Traffic Analysis

Use GitHub Insights:
- Repository > Insights > Traffic
- See views, unique visitors, referring sites

### User Feedback

Collect feedback via:
- GitHub Issues
- Google Forms
- Email (add contact info)

## 🔒 Security

### GitHub Pages Security

- **HTTPS**: Automatic (enforced by GitHub)
- **DDoS Protection**: Built-in
- **Access Control**: Repository visibility settings

### Content Security

- Don't commit sensitive data
- No API keys in code
- No proprietary data without permission
- Review before making repository public

## 🆘 Getting Help

If you encounter issues:

1. **Docsify Documentation**: [docsify.js.org](https://docsify.js.org/)
2. **GitHub Pages Docs**: [docs.github.com/pages](https://docs.github.com/pages)
3. **Community**:
   - Stack Overflow: Tag `docsify`
   - GitHub Discussions
   - Docsify Gitter

## 🎓 Advanced Topics

### Custom Plugins

Add custom Docsify plugins in `index.html`:

```html
<script>
  window.$docsify = {
    // ... config
    plugins: [
      function(hook, vm) {
        // Your custom plugin code
      }
    ]
  };
</script>
```

### Build Pipeline

For advanced builds (preprocessing, etc.):

```bash
# Install dependencies
npm init -y
npm install docsify-cli --save-dev

# Add to package.json
{
  "scripts": {
    "serve": "docsify serve .",
    "deploy": "npm run build && ./deploy.sh"
  }
}
```

### Internationalization

Support multiple languages:
```
docs/
  ├── README.md (English)
  ├── zh-cn/
  │   └── README.md (Chinese)
  └── vi/
      └── README.md (Vietnamese)
```

Configure in `index.html`:
```javascript
window.$docsify = {
  loadSidebar: '_sidebar.md',
  alias: {
    '/.*/_sidebar.md': '/_sidebar.md'
  },
  // ... other config
};
```

---

## ✅ Deployment Complete!

Your Vietnam Market Study documentation is now live and accessible to the world.

**Next Steps**:
1. Share the URL with colleagues
2. Start filling in template sections
3. Keep content updated
4. Gather feedback
5. Iterate and improve

**Questions?** Open an issue in the repository or refer to the main README.

---

**Happy documenting! 📚**
