# GitHub Pages Deployment Guide

This guide will help you deploy your portfolio website to GitHub Pages for free.

## Prerequisites
- A GitHub account (create one at [github.com](https://github.com) if you don't have one)
- Git installed on your computer ([Download Git](https://git-scm.com/downloads))
- Your portfolio files ready in the `port` folder

## Step-by-Step Instructions

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the **"+"** icon in the top right corner
3. Select **"New repository"**
4. Fill in the repository details:
   - **Repository name**: `rohith-portfolio` (or any name you prefer)
   - **Description**: "My Portfolio Website"
   - **Visibility**: Choose **Public** (required for free GitHub Pages)
   - **DO NOT** initialize with README, .gitignore, or license
5. Click **"Create repository"**

### Step 2: Initialize Git in Your Portfolio Folder

Open your terminal/command prompt and navigate to your portfolio folder:

**For Windows (PowerShell):**
```powershell
cd D:\code\port
git init
```

**For Mac/Linux:**
```bash
cd /path/to/port
git init
```

### Step 3: Add All Files to Git

```bash
git add .
```

### Step 4: Commit Your Files

```bash
git commit -m "Initial commit - Portfolio website"
```

### Step 5: Connect to GitHub Repository

Replace `YOUR_USERNAME` with your actual GitHub username:

```bash
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/rohith-portfolio.git
```

For example, if your username is `RH1H`:
```bash
git remote add origin https://github.com/RH1H/rohith-portfolio.git
```

### Step 6: Push Your Code to GitHub

```bash
git push -u origin main
```

You'll be prompted for your GitHub username and password. If you have two-factor authentication enabled, use a Personal Access Token instead of your password.

**To create a Personal Access Token:**
1. Go to GitHub Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Click "Generate new token (classic)"
3. Give it a name and select `repo` scope
4. Copy the token and use it as your password when pushing

### Step 7: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **"Settings"** tab (at the top of the repository)
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Source"**, select:
   - Branch: **`main`**
   - Folder: **`/ (root)`**
5. Click **"Save"**

### Step 8: Access Your Live Website

After a few minutes, your website will be live at:
```
https://YOUR_USERNAME.github.io/rohith-portfolio/
```

For example: `https://RH1H.github.io/rohith-portfolio/`

## Updating Your Website

Whenever you make changes to your portfolio:

```bash
git add .
git commit -m "Update portfolio - describe your changes"
git push
```

Your changes will be live on GitHub Pages within 1-2 minutes.

## Quick Command Summary

```bash
# Navigate to your portfolio folder
cd D:\code\port

# Initialize git (only first time)
git init

# Add all files
git add .

# Commit changes
git commit -m "Your commit message"

# Connect to GitHub (only first time - replace YOUR_USERNAME)
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/rohith-portfolio.git

# Push to GitHub
git push -u origin main
```

## Troubleshooting

### Issue: "Repository not found"
- Make sure you've created the repository on GitHub first
- Check that the repository name matches exactly
- Verify your username is correct

### Issue: "Authentication failed"
- Use a Personal Access Token instead of password
- Make sure you have write access to the repository

### Issue: Website shows 404
- Wait 1-2 minutes after enabling GitHub Pages
- Check that you selected the correct branch (`main`) and folder (`/ (root)`)
- Make sure `index.html` is in the root folder

### Issue: Images not loading
- Make sure image paths use relative paths (e.g., `images/rohith.jpg`)
- Don't use absolute paths like `C:\...` or `/Users/...`
- All paths should be relative to the root folder

## Custom Domain (Optional)

If you have a custom domain:

1. Create a file named `CNAME` in your repository root
2. Add your domain name (e.g., `www.yourname.com`) in the file
3. Configure DNS settings with your domain provider:
   - Add a CNAME record pointing to `YOUR_USERNAME.github.io`

## Additional Tips

- Your repository will be public (required for free GitHub Pages)
- Changes may take 1-2 minutes to appear on the live site
- You can check the deployment status in the "Actions" tab
- Always test your site locally before pushing changes

---

**Need Help?** Check GitHub Pages documentation: https://docs.github.com/en/pages

