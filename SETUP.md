# 🚀 Setup & Hosting Guide

## Folder Structure

```
your-username/          ← GitHub repo named exactly your GitHub username
├── README.md           ← Main profile file
└── assets/
    ├── hero-banner.svg     ← Animated hero banner
    ├── tech-domains.svg    ← Tech stack domain cards
    ├── projects.svg        ← Project terminal cards
    └── philosophy.svg      ← Engineering philosophy grid
```

## Step-by-Step Deployment

### 1. Create the Special Profile Repository
- Go to github.com → New repository
- Name it **exactly** your GitHub username: `mshahnawaz1202`
- Set to **Public**
- Do NOT initialize with a README (you'll add your own)

### 2. Clone and Add Files
```bash
git clone https://github.com/mshahnawaz1202/mshahnawaz1202.git
cd mshahnawaz1202
mkdir assets

# Copy all files from this package into the folder
# README.md  →  root
# *.svg      →  assets/
```

### 3. Push to GitHub
```bash
git add .
git commit -m "feat: cyberpunk engineering profile dashboard"
git push origin main
```

### 4. Verify
Visit `github.com/mshahnawaz1202` — your profile README renders automatically.

---

## SVG Hosting Notes

All SVGs use **relative paths** (`./assets/filename.svg`) which work natively
when the files are in the same repo. GitHub renders SVGs inline in READMEs.

**No external hosting needed.** GitHub serves the SVGs directly.

---

## Customization Quick Reference

| What to change | Where | How |
|:---|:---|:---|
| Name / tagline | `hero-banner.svg` | Edit `<text>` elements |
| Skill bar lengths | `tech-domains.svg` | Change `to="NNN"` in `<animate>` |
| Project descriptions | `projects.svg` | Edit `<text>` content |
| GitHub stats theme | `README.md` | Change `theme=` param in URL |
| Contact links | `README.md` | Replace URLs in `href=` |

---

## Verified Compatible With
- ✅ GitHub Dark theme
- ✅ GitHub Light theme  
- ✅ GitHub Dimmed theme
- ✅ Mobile GitHub app
- ✅ All modern browsers
