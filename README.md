# Frames by Sunanda — Photography Portfolio

A premium, cinematic photography portfolio website for luxury brand **Frames by Sunnada** by Sunnada Kommadi.

---

## 📁 Folder Structure

```
frames-by-sunnada/
├── index.html          # Main website (self-contained)
├── README.md           # This file
└── assets/             # (optional) for your own photos
    ├── images/
    │   ├── hero/       # Full-screen hero slideshow images
    │   ├── portfolio/  # Gallery images
    │   ├── about/      # Photographer portrait
    │   └── featured/   # Featured work section images
    └── favicon.ico
```

> The site is **100% self-contained in `index.html`** — no build tools, no dependencies to install. Just open in a browser or deploy.

---

## 🚀 Deploy to GitHub Pages (Free)

### Step 1 — Create a GitHub Repository
1. Go to [github.com](https://github.com) → **New Repository**
2. Name it: `frames-by-sunnada` (or `your-username.github.io` for a root domain)
3. Set to **Public**, click **Create Repository**

### Step 2 — Upload Your Files
**Option A — Via GitHub Web UI (easiest):**
1. Open your new repository
2. Click **Add file → Upload files**
3. Drag `index.html` (and any assets) → **Commit changes**

**Option B — Via Git CLI:**
```bash
git init
git add .
git commit -m "Initial commit — Frames by Sunnada"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/frames-by-sunnada.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages
1. Go to your repo → **Settings** → **Pages** (left sidebar)
2. Under **Source**, select **Deploy from a branch**
3. Branch: `main`, Folder: `/ (root)` → **Save**
4. Your site will be live at:  
   `https://YOUR_USERNAME.github.io/frames-by-sunnada/`

### Step 4 — Custom Domain (Optional)
1. Buy a domain (e.g., `framesbysunnada.com`) from Namecheap or Google Domains
2. In GitHub Pages settings → **Custom domain** → enter your domain
3. Add a `CNAME` file to your repo containing your domain name
4. Update your domain's DNS: add a CNAME record pointing to `YOUR_USERNAME.github.io`

---

## 🖼️ Replacing Demo Images with Your Own Photos

The site currently uses **Unsplash placeholder images**. To use your own:

1. Place photos in `/assets/images/`
2. In `index.html`, find the image URLs (search for `unsplash.com`)
3. Replace each URL with your local path, e.g.:
   ```html
   <!-- Before -->
   <img src="https://images.unsplash.com/photo-xxxx?w=800" />
   <!-- After -->
   <img src="assets/images/portfolio/wedding-01.jpg" />
   ```

### Recommended Image Specs
| Section | Size | Format |
|---------|------|--------|
| Hero slides | 1800×1200px | JPG (quality 85) |
| Portfolio grid | 800×1000px | JPG (quality 80) |
| Featured work | 1200×900px | JPG (quality 85) |
| About portrait | 800×1000px | JPG (quality 85) |

---

## ✨ Tips to Make It Award-Winning

### 1. **Photography Quality is Everything**
- Use your **absolute best 9–12 images** in the portfolio grid
- Ensure color grading is **consistent** across all photos (same LUT/preset)
- Hero slides: use **wide, dramatic landscape shots** with strong mood

### 2. **Typography Refinement**
- The site uses **Cormorant Garamond** (serif) + **Jost** (sans) — a luxury pairing
- If you want more edge: swap Cormorant for **Playfair Display** or **Editorial New**

### 3. **Performance Optimizations**
```bash
# Compress images (install: npm install -g sharp-cli)
sharp input.jpg -o output.jpg -q 80 --resize 1800

# Or use squoosh.app (free, browser-based)
```
- Use **WebP format** instead of JPG for 30–40% smaller files
- Add `loading="lazy"` to all below-fold images (already done ✓)

### 4. **SEO Improvements**
Update the `<head>` section:
```html
<meta property="og:image" content="https://yoursite.com/assets/images/og-preview.jpg" />
<link rel="canonical" href="https://framesbysunnada.com" />
```
Add a `sitemap.xml` and submit to Google Search Console.

### 5. **Advanced Animations (optional upgrade)**
Install GSAP for cinematic scroll animations:
```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollTrigger.min.js"></script>
```

### 6. **Contact Form Backend**
The form currently shows a visual confirmation. To receive real emails:
- **Formspree** (free): Replace `<form>` action with `https://formspree.io/f/YOUR_ID`
- **EmailJS**: Add their SDK and connect to Gmail
- **Netlify Forms**: Deploy on Netlify instead of GitHub Pages for free form handling

### 7. **Analytics**
Add Google Analytics or Plausible to track visitors:
```html
<!-- Plausible (privacy-friendly) -->
<script defer data-domain="framesbysunnada.com" src="https://plausible.io/js/script.js"></script>
```

---

## 🎨 Brand Color Reference

| Name | Hex | Usage |
|------|-----|-------|
| Black | `#0a0a0a` | Background |
| Charcoal | `#141414` | Section backgrounds |
| White | `#f5f2ee` | Body text |
| Gold | `#c9a96e` | Accents, CTAs |
| Gold Light | `#e2c89a` | Italic highlights |

---

## 📞 Support

For customizations, reach out or modify `index.html` directly — everything is in one file and well-commented.

© 2026 Sunnada Kommadi — Frames by Sunnada
