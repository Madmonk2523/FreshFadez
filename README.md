# Fresh Fadez Barbershop 💈

A modern, responsive single-page website for Fresh Fadez Barbershop in Phoenix, Arizona.

## 🔥 About Fresh Fadez

Fresh Fadez is a premium barbershop located in Phoenix, AZ, specializing in all haircuts and hair types. With over 20 years of experience, our expert barbers provide exceptional service including:

- All haircut styles and types
- Custom designs and patterns
- Beard styling and maintenance
- Hair enhancements
- Great for kids
- Walk-ins welcome

**Location:** 2637 W Bethany Home Rd, Phoenix, AZ 85017  
**Phone:** (602) 374-3339  
**Booking:** [Book Online via Squire](https://getsquire.com/booking/book/fresh-fadez-barbershop-phoenix)

### Business Hours

| Day | Hours |
|-----|-------|
| Monday | 9 AM – 7 PM |
| Tuesday | 9 AM – 7 PM |
| Wednesday | 9 AM – 7 PM |
| Thursday | 9 AM – 7 PM |
| Friday | 9 AM – 7 PM |
| Saturday | 9 AM – 6 PM |
| Sunday | 10 AM – 4 PM |

## 🌐 Website Features

- **Premium Dark Theme** - Sophisticated charcoal, gold, and white color scheme
- **Fully Responsive** - Mobile-first design that works on all devices
- **Sticky Navigation** - Always accessible menu with Book Now button
- **Interactive Elements:**
  - Smooth scrolling
  - Hamburger mobile menu
  - FAQ accordion
  - Floating mobile Book Now button
  - IntersectionObserver animations
- **Accessibility:**
  - ARIA labels
  - Keyboard navigation
  - Focus states
  - Skip links
- **SEO Optimized:**
  - Meta tags
  - Open Graph tags
  - JSON-LD structured data
  - Semantic HTML
- **Sections:**
  - Hero with CTAs
  - Highlights
  - About
  - Hours & Google Maps
  - Customer Reviews
  - FAQ
  - Social Links
  - Footer

## 🚀 Deployment Instructions

### Option 1: GitHub Pages (Recommended for GitHub hosting)

GitHub Pages is perfect for hosting static websites directly from your GitHub repository.

1. **Push to GitHub** (see Git Setup section below)

2. **Enable GitHub Pages:**
   - Go to your repository on GitHub: `https://github.com/Madmonk2523/FreshFadez`
   - Click **Settings**
   - Scroll to **Pages** in the left sidebar
   - Under **Source**, select `main` branch
   - Click **Save**

3. **View Your Site:**
   - Your site will be live at: `https://madmonk2523.github.io/FreshFadez/`
   - It may take 2-3 minutes for the initial deployment

4. **Custom Domain (Optional):**
   - Purchase a domain (e.g., freshfadez.com)
   - In GitHub Pages settings, add your custom domain
   - Update your domain's DNS settings:
     - Add a CNAME record pointing to `madmonk2523.github.io`
     - Or add A records pointing to GitHub's IPs

### Option 2: Netlify (Recommended for CI/CD)

Netlify offers automatic deployments, SSL certificates, and form handling.

1. **Connect Repository:**
   - Go to [netlify.com](https://www.netlify.com/)
   - Click **Add new site** → **Import an existing project**
   - Choose **GitHub** and authorize Netlify
   - Select the `FreshFadez` repository

2. **Configure Build Settings:**
   - Build command: *(leave empty)*
   - Publish directory: `/` *(default)*
   - Click **Deploy site**

3. **View Your Site:**
   - Netlify will provide a URL like: `https://freshfadez.netlify.app`
   - Every push to `main` branch auto-deploys

4. **Custom Domain:**
   - Go to **Site settings** → **Domain management**
   - Click **Add custom domain**
   - Follow the instructions to update your DNS settings

**Netlify Features:**
- Free SSL certificates
- Automatic deployments on git push
- Branch previews
- Form handling (if you add forms later)

### Option 3: Vercel (Recommended for modern hosting)

Vercel provides fast global CDN and excellent developer experience.

1. **Import Repository:**
   - Go to [vercel.com](https://vercel.com/)
   - Click **Add New** → **Project**
   - Import your GitHub repository: `FreshFadez`

2. **Configure Project:**
   - Framework Preset: **Other**
   - Root Directory: `./`
   - Build Command: *(leave empty)*
   - Output Directory: `./`
   - Click **Deploy**

3. **View Your Site:**
   - Vercel provides a URL like: `https://fresh-fadez.vercel.app`
   - Automatic deployments on every push

4. **Custom Domain:**
   - Go to **Settings** → **Domains**
   - Add your custom domain
   - Update DNS according to Vercel's instructions

**Vercel Features:**
- Edge network for fast loading worldwide
- Automatic HTTPS
- Preview deployments for pull requests
- Analytics (with paid plans)

## 🔧 Git Setup & GitHub Push

Follow these commands to initialize the repository and push to GitHub:

```powershell
# Navigate to project directory
cd "c:\Users\chase\OneDrive\Desktop\DigitalWebServices\FreshFadez"

# Initialize Git repository
git init

# Add all files to staging
git add .

# Create initial commit
git commit -m "Initial commit: Fresh Fadez Barbershop website"

# Add GitHub remote
git remote add origin https://github.com/Madmonk2523/FreshFadez.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

### Authentication

If prompted for credentials:

**Option 1: GitHub CLI (Recommended)**
```powershell
# Install GitHub CLI
winget install --id GitHub.cli

# Authenticate
gh auth login

# Then retry the push
```

**Option 2: Personal Access Token**
1. Go to GitHub → Settings → Developer settings → Personal access tokens
2. Generate new token (classic) with `repo` scope
3. Use token as password when prompted

**Option 3: SSH Key**
```powershell
# Generate SSH key
ssh-keygen -t ed25519 -C "your_email@example.com"

# Add to ssh-agent
ssh-add ~/.ssh/id_ed25519

# Copy public key
cat ~/.ssh/id_ed25519.pub

# Add to GitHub → Settings → SSH Keys

# Update remote to use SSH
git remote set-url origin git@github.com:Madmonk2523/FreshFadez.git
```

## 📁 Project Structure

```
FreshFadez/
├── index.html          # Complete website (HTML + CSS + JS)
├── README.md          # This file
└── .gitignore         # Git ignore rules
```

## 🔄 Future Updates

To update the website:

1. **Edit Files:**
   ```powershell
   # Make changes to index.html or other files
   ```

2. **Commit & Push:**
   ```powershell
   git add .
   git commit -m "Update: description of changes"
   git push
   ```

3. **Automatic Deployment:**
   - GitHub Pages: Automatically rebuilds
   - Netlify: Automatically deploys on push
   - Vercel: Automatically deploys on push

## 🛠️ Customization

### Update Business Information

Edit the following in `index.html`:

- **Contact Info:** Lines 20-40 (meta tags and JSON-LD)
- **Phone Number:** Search for `(602) 374-3339` and replace
- **Address:** Search for `2637 W Bethany Home Rd` and replace
- **Social Links:** Search for Instagram/Facebook URLs and replace
- **Booking Link:** Search for `getsquire.com` URL and replace

### Update Colors

Edit CSS variables in `index.html` (around line 50):

```css
:root {
    --color-charcoal: #1a1a1a;
    --color-gold: #d4af37;
    --color-white: #ffffff;
    /* ... other colors */
}
```

### Update Hours

Edit the hours section in `index.html` (search for "Business Hours")

## 📱 Social Links

- **Instagram:** [freshfadezbarbershop](https://www.instagram.com/freshfadezbarbershop/)
- **Facebook:** [freshfadez](https://www.facebook.com/freshfadez/)
- **Book Online:** [Squire Booking](https://getsquire.com/booking/book/fresh-fadez-barbershop-phoenix)

## 📄 License

© 2026 Fresh Fadez Barbershop. All rights reserved.

## 💡 Technical Support

For questions or assistance with the website:
- Check deployment platform documentation
- Review browser console for errors
- Verify all links and phone numbers are working
- Test on multiple devices and browsers

---

**Built with:** HTML5, CSS3, JavaScript  
**Optimized for:** SEO, Performance, Accessibility  
**Compatible with:** All modern browsers
