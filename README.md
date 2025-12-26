# MeetNicoleJolie.com - AI Trust Signal Audit Landing Page

Professional landing page for AI Trust Signal Audit services targeting high-value B2B companies in insurance, lending, capital raising, and industrial services.

## 🚀 Quick Deploy to GitHub Pages

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and log in
2. Click the **+** icon (top right) → **New repository**
3. Repository name: `meetnicolejolie`
4. Set to **Public** (required for free GitHub Pages)
5. Do NOT initialize with README (we already have one)
6. Click **Create repository**

### Step 2: Upload Files

**Option A: Via GitHub Web Interface (Easiest)**

1. In your new repository, click **uploading an existing file**
2. Drag and drop these files:
   - `index.html`
   - `README.md`
3. Create folder structure by typing in the file upload area:
   - `css/styles.css` (type `css/styles.css` then upload the file)
4. Scroll down and click **Commit changes**

**Option B: Via Git Command Line**
```bash
# Navigate to your project folder
cd /path/to/meetnicolejolie

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: AI Trust Signal Audit landing page"

# Add remote (replace USERNAME with your GitHub username)
git remote add origin https://github.com/USERNAME/meetnicolejolie.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. In your repository, go to **Settings**
2. Scroll down to **Pages** (in left sidebar)
3. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**
5. Wait 2-3 minutes for deployment
6. Your site will be live at: `https://USERNAME.github.io/meetnicolejolie/`

### Step 4: Add Custom Domain (Optional)

If you want to use `meetnicolejolie.com` instead of the GitHub URL:

1. In your domain registrar (Namecheap), add these DNS records:
```
   Type: A
   Host: @
   Value: 185.199.108.153
   
   Type: A
   Host: @
   Value: 185.199.109.153
   
   Type: A
   Host: @
   Value: 185.199.110.153
   
   Type: A
   Host: @
   Value: 185.199.111.153
   
   Type: CNAME
   Host: www
   Value: USERNAME.github.io
```

2. In GitHub Pages settings, enter custom domain: `meetnicolejolie.com`
3. Wait 24-48 hours for DNS propagation
4. Enable **Enforce HTTPS** (recommended)

---

## 📁 File Structure
```
meetnicolejolie/
├── index.html          # Main landing page (all content)
├── css/
│   └── styles.css      # All styling
└── README.md           # This file (deployment instructions)
```

---

## 🎨 Customization Guide

### Update Images

All images are hosted on AWS S3. To change images:

1. Upload new image to your S3 bucket: `nicolejoliewebsite`
2. Make it public
3. Copy the S3 URL
4. Find the image reference in `index.html` (search for the old URL)
5. Replace with new URL

**Current image locations in index.html:**

- **Hero image**: Line 295
```html
  <img src="https://meetnicolejolie.s3.us-east-2.amazonaws.com/header_image_meetnj_desktop.png"
```

- **Trust Signal Gaps graphic**: Line 376
```html
  <img src="https://meetnicolejolie.s3.us-east-2.amazonaws.com/Graphic+5+-+Trust+Signal+Gaps+the+invisible+revenue+leak.png"
```

- **Cost Comparison Table**: Line 415
```html
  <img src="https://meetnicolejolie.s3.us-east-2.amazonaws.com/Graphic+4-+The+Cost+Comparison+Table.png"
```

- **3-Step Process**: Line 476
```html
  <img src="https://meetnicolejolie.s3.us-east-2.amazonaws.com/Graphic+3-+Trust+Signal+Breakdown+-+Before+%26+After.png"
```

### Update CTA Links

All "Book Your AI Trust Signal Audit" buttons link to Google Calendar.

**Current link**: `https://calendar.app.google/7pga1PerT94ZCuZq6`

To update, search `index.html` for `calendar.app.google` and replace all instances with your new booking link.

**Button locations:**
- Header navigation: Line 276
- Hero section: Line 290
- What Happens Next: Line 570
- Final CTA: Line 737

### Update Copy

All copy is in `index.html`. To edit:

1. Open `index.html` in any text editor
2. Find the section you want to change
3. Edit the text between HTML tags
4. Save and push to GitHub

**Do NOT change:**
- HTML structure tags (`<div>`, `<section>`, `<p>`, etc.)
- CSS class names (`class="hero"`, etc.)
- Schema markup in `<head>` section

### Update Colors

Colors are defined in `css/styles.css`. Current palette:
```css
/* Main Colors */
--dark-navy: #001524;      /* Text, headers */
--teal: #15616d;           /* Buttons, accents */
--cream: #ffecd1;          /* Section backgrounds */
--white: #ffffff;          /* Main background */
```

To change colors:

1. Open `css/styles.css`
2. Search for the color hex code you want to change
3. Replace with new hex code
4. Save and push to GitHub

**Example: Change teal to purple**
- Find all instances of `#15616d`
- Replace with `#7c3aed` (purple)

### Update Fonts

Current fonts:
- **Headings**: Montserrat (bold, sans-serif)
- **Body**: EB Garamond (serif)

To change fonts:

1. Go to [Google Fonts](https://fonts.google.com)
2. Select your fonts
3. Copy the import code
4. In `css/styles.css`, replace line 7:
```css
   @import url('YOUR_NEW_GOOGLE_FONTS_URL');
```
5. Update font-family references throughout the CSS

---

## 🔧 Technical Details

### Performance Optimizations

- **No JavaScript dependencies**: Pure HTML/CSS (fast load times)
- **Optimized images**: All graphics hosted on AWS S3 with CDN
- **Minimal CSS**: Single stylesheet, no frameworks
- **Mobile-first responsive**: Works perfectly on all devices

### Browser Compatibility

Tested and working on:
- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

### SEO & AI Crawling

**Comprehensive Schema.org markup includes:**
- Person (Nicole Jolie as AI Search Consultant)
- Organization (Worthy of Success LLC)
- ProfessionalService (AI Trust Signal Audit)
- WebPage (Landing page metadata)
- FAQPage (All 10 FAQs structured for AI)
- BreadcrumbList (Site navigation)

**AI systems that can crawl this page:**
- ChatGPT / OpenAI
- Google AI Overviews
- Gemini
- Claude (Anthropic)
- Perplexity
- DeepSeek
- Any LLM with web crawling capabilities

### Page Speed

Target metrics:
- First Contentful Paint: < 1.5s
- Largest Contentful Paint: < 2.5s
- Time to Interactive: < 3.5s

**To test your page speed:**
1. Go to [PageSpeed Insights](https://pagespeed.web.dev/)
2. Enter your URL
3. Click **Analyze**

---

## 📝 Content Updates

### Adding a New FAQ

1. Open `index.html`
2. Find the FAQ section (starts around line 580)
3. Copy an existing `<div class="faq-item">` block
4. Paste it before the closing `</div>` of `faq-container`
5. Update the question and answer text
6. Update the schema markup in `<head>` (lines 100-250) to include the new FAQ

### Changing Scenario Dollar Amounts

Find the scenarios grid (lines 308-369). Each scenario has:
```html
<span class="scenario-dollar">$150,000</span>
```

Update the number to match your new calculations.

### Updating Footer Links

Footer starts at line 753. To add/remove legal pages:

1. Find the footer nav section
2. Add or remove `<a href="...">` links
3. Make sure the linked HTML files exist in your repository

---

## 🐛 Troubleshooting

### Page not showing up after deploy

**Wait 3-5 minutes** after enabling GitHub Pages. Deployment is not instant.

If still not working:
1. Check **Settings → Pages** shows a green checkmark
2. Verify branch is set to `main` and folder is `/ (root)`
3. Check repository is **Public** (not Private)

### Images not loading

1. **Check S3 URLs are correct** in `index.html`
2. **Verify images are public** in AWS S3 console
3. Test URL directly in browser (should download/display image)

### Styles not applying

1. **Check file path**: `css/styles.css` must be in a folder called `css`
2. **Check line 263 in index.html**: `<link rel="stylesheet" href="css/styles.css">`
3. **Case sensitive**: Make sure folder is lowercase `css` not `CSS`

### Custom domain not working

1. **Wait 24-48 hours** for DNS propagation
2. **Check DNS records** at [whatsmydns.net](https://whatsmydns.net)
3. **Verify A records** point to GitHub's IPs (listed above)
4. **Check CNAME** points to `USERNAME.github.io`

### Mobile layout broken

1. **Check viewport meta tag** exists in `<head>` (line 256)
2. **Test responsive breakpoints** in browser DevTools
3. **Verify CSS media queries** in `styles.css` (lines 500+)

---

## 🔄 Making Updates After Launch

### Quick Text Edits

1. Go to your GitHub repository
2. Click `index.html`
3. Click the **pencil icon** (Edit this file)
4. Make your changes
5. Scroll down → **Commit changes**
6. Wait 2-3 minutes for GitHub Pages to rebuild
7. Refresh your live site

### Larger Updates

1. Clone repository to your computer:
```bash
   git clone https://github.com/USERNAME/meetnicolejolie.git
```

2. Make changes in your text editor

3. Push updates:
```bash
   git add .
   git commit -m "Describe your changes"
   git push
```

4. GitHub Pages auto-deploys in 2-3 minutes

---

## 📊 Analytics Setup (Optional)

### Add Google Analytics

1. Get your GA4 tracking code from Google Analytics
2. Add this to `index.html` before the closing `</head>` tag:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

Replace `G-XXXXXXXXXX` with your actual GA4 ID.

---

## 📞 Support

### Common Questions

**Q: Can I use this with my own domain?**
A: Yes. Follow Step 4 in Quick Deploy section.

**Q: Do I need to know how to code?**
A: No. All code is ready to use. Just follow deployment steps.

**Q: How do I update the booking link?**
A: Search `index.html` for the old Google Calendar URL and replace with new one.

**Q: Can I change the colors?**
A: Yes. Edit hex codes in `css/styles.css`.

**Q: Will this work on mobile?**
A: Yes. Fully responsive design tested on all devices.

### Need Help?

If you run into issues:

1. Check the troubleshooting section above
2. Review GitHub Pages documentation: [docs.github.com/pages](https://docs.github.com/pages)
3. Test in incognito browser (clears cache issues)

---

## 📄 License

Copyright © 2025 Worthy of Success LLC. All rights reserved.

---

## ✅ Launch Checklist

Before going live:

- [ ] All images uploaded to S3 and public
- [ ] Image URLs updated in `index.html`
- [ ] Calendar booking link updated in all CTAs
- [ ] Footer legal pages created (or links removed)
- [ ] Schema markup reviewed (correct URLs, dates)
- [ ] Tested on desktop browser
- [ ] Tested on mobile device
- [ ] Page speed tested (PageSpeed Insights)
- [ ] All links working (no 404s)
- [ ] Spelling and grammar checked
- [ ] Google Analytics added (optional)
- [ ] Custom domain configured (if using)

---

**Your landing page is ready to deploy. Follow the Quick Deploy steps above and you'll be live in under 10 minutes.**

**Questions? Review the troubleshooting section or GitHub Pages documentation.**
