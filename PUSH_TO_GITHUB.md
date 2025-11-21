# Quick Guide: Push Your Code to GitHub

## Step 1: Create GitHub Repository (Do this first!)

1. Go to https://github.com and sign in
2. Click the **"+"** icon (top right) → **"New repository"**
3. Repository name: `kiraneeb` (or any name you like)
4. Description: "Personal website"
5. Make it **Public** ✅ (required for free GitHub Pages)
6. **DO NOT** check any boxes (no README, .gitignore, or license)
7. Click **"Create repository"**

## Step 2: Copy Your Repository URL

After creating the repo, GitHub will show you a page with commands. 
**Your repository URL will be:**
```
https://github.com/kiraneeb/kiraneeb.git
```

## Step 3: Run These Commands in Terminal

Open Terminal (Applications → Utilities → Terminal) and copy/paste these commands one by one:

```bash
# Navigate to your project
cd /Users/kiraneeb/Desktop/misproject1

# Initialize git repository
git init

# Add all your files
git add .

# Create your first commit
git commit -m "Initial commit: Personal website"

# Add your GitHub repository
git remote add origin https://github.com/kiraneeb/kiraneeb.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub (you'll be asked for your GitHub username and password/token)
git push -u origin main
```

## Important Notes:

- When you run `git push`, you'll need to authenticate:
  - **Username**: Your GitHub username
  - **Password**: Use a **Personal Access Token** (not your password)
    - Get one here: https://github.com/settings/tokens
    - Click "Generate new token (classic)"
    - Select scope: `repo`
    - Copy the token and use it as your password

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Click **Pages** (left sidebar)
4. Under "Source", select **"Deploy from a branch"**
5. Branch: **main**, Folder: **/ (root)**
6. Click **Save**

Your site will be live at: `https://kiraneeb.github.io/kiraneeb/`

## Need Help?

If you get errors, make sure:
- You've created the GitHub repository first (named 'kiraneeb')
- You're using a Personal Access Token (not your password)

