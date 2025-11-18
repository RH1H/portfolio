# Quick Deployment Guide - GitHub Pages

## Fastest Method (Copy-Paste Commands)

### Step 1: Open PowerShell/Terminal in your portfolio folder

**Windows (PowerShell):**
1. Navigate to `D:\code\port` folder
2. Right-click and select "Open in Terminal" or "Open PowerShell window here"

### Step 2: Run these commands one by one

Replace `YOUR_USERNAME` with your GitHub username (e.g., `RH1H`)
Replace `YOUR_REPO_NAME` with your repository name (e.g., `rohith-portfolio`)

```powershell
# Initialize Git
git init

# Add all files
git add .

# Commit files
git commit -m "Deploy portfolio website"

# Set branch to main
git branch -M main

# Add GitHub remote (replace YOUR_USERNAME and YOUR_REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Push to GitHub
git push -u origin main
```

**Example:**
If your username is `RH1H` and repo name is `rohith-portfolio`:
```powershell
git remote add origin https://github.com/RH1H/rohith-portfolio.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository: `https://github.com/YOUR_USERNAME/YOUR_REPO_NAME`
2. Click **Settings** tab
3. Click **Pages** in left sidebar
4. Under **Source**:
   - Select branch: **`main`**
   - Select folder: **`/ (root)`**
5. Click **Save**

### Step 4: Access Your Website

Your site will be live at:
```
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/
```

**Example:**
```
https://RH1H.github.io/rohith-portfolio/
```

---

## Alternative: Use the Deployment Script

1. Open PowerShell in the `port` folder
2. Run:
   ```powershell
   .\deploy.ps1
   ```
3. Follow the prompts

---

## Common Issues

### Authentication Failed
If you get an authentication error:
1. Go to: https://github.com/settings/tokens
2. Click "Generate new token (classic)"
3. Give it a name, select `repo` scope
4. Copy the token
5. Use the token as your password when pushing

### Repository Not Found
- Make sure you created the repository on GitHub first
- Check that the name matches exactly (case-sensitive)

### First Time Setup
If this is your first time using Git:
```powershell
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

---

**That's it! Your portfolio will be live in 1-2 minutes.**

