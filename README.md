# The Drilling Lab — Website

A minimal, editorial one-page landing site for The Drilling Lab consulting.

## Local Preview

**Option A: VS Code Live Server**
1. Install the "Live Server" extension in VS Code
2. Right-click `index.html` → "Open with Live Server"

**Option B: Python HTTP Server**
```bash
# Navigate to project folder
cd "C:\Users\kurtw\OneDrive - Fatskn\THE_DRILLING_LAB_WEBSITE"

# Start server (Python 3)
python -m http.server 8000

# Open http://localhost:8000 in your browser
```

---

## GitHub Pages Deployment

### 1. Initialize Git & Push to GitHub

```bash
# Navigate to project folder
cd "C:\Users\kurtw\OneDrive - Fatskn\THE_DRILLING_LAB_WEBSITE"

# Initialize git repository
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: The Drilling Lab website"

# Add your GitHub repo as remote (replace with your repo URL)
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# Push to main branch
git branch -M main
git push -u origin main
```

### 2. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under "Source", select:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Click **Save**

### 3. Find Your Live URL

After a few minutes, your site will be live at:
```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

This URL appears in the GitHub Pages settings once deployment completes.

---

## Custom Domain (Optional)

To connect a custom domain (e.g., from GoDaddy):

1. **In GitHub:**
   - Go to Settings → Pages
   - Under "Custom domain", enter your domain (e.g., `thedrillinglab.com`)
   - Check "Enforce HTTPS"

2. **In GoDaddy DNS:**
   - Add an **A record** pointing to GitHub Pages IPs:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - Add a **CNAME record** for `www` pointing to `YOUR-USERNAME.github.io`

3. Wait for DNS propagation (can take up to 48 hours)

---

## Files

```
THE_DRILLING_LAB_WEBSITE/
├── index.html      # Main HTML page
├── style.css       # Stylesheet
├── README.md       # This file
└── .gitignore      # Git ignore rules
```

---

## Placeholders to Update

Before publishing, edit `index.html` and replace:

- `https://calendly.com/YOUR-LINK-HERE` → Your actual Calendly link
- `YOUR-EMAIL@DOMAIN.COM` → Your contact email
- `[Founder Name]` → Founder's name
- `[XX] years` → Years of experience
- `[industry / function]` → Industry or function description
- `[Company A]` and `[Company B]` → Previous companies
- `[City]` → Your city/location

---

© The Drilling Lab
