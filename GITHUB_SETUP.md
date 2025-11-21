# GitHub Pages Setup Instructions

Your project is now ready for GitHub Pages! Follow these steps to deploy it:

## Step 1: Install Git (if needed)

If you see an error about Xcode command line tools, install them:
```bash
xcode-select --install
```

## Step 2: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon in the top right → "New repository"
3. Repository name: `kiraneeb` (or any name you prefer)
4. Description: "Personal website"
5. Make it **Public** (required for free GitHub Pages)
6. **DO NOT** initialize with README, .gitignore, or license (we already have these)
7. Click "Create repository"

## Step 3: Connect and Push Your Code

Open Terminal and run these commands (replace `YOUR_USERNAME` with your GitHub username):

```bash
cd /Users/kiraneeb/Desktop/misproject1

# Initialize git (if not already done)
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit: Personal website"

# Add your GitHub repository as remote
git remote add origin https://github.com/kiraneeb/kiraneeb.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Scroll down to **Pages** (left sidebar)
4. Under "Source", select **"Deploy from a branch"**
5. Select branch: **main**
6. Select folder: **/ (root)**
7. Click **Save**

## Step 5: Access Your Live Website

After a few minutes, your website will be live at:
- **https://kiraneeb.github.io/kiraneeb/**

## Updating Your Website

Whenever you make changes:

```bash
cd /Users/kiraneeb/Desktop/misproject1
git add .
git commit -m "Description of your changes"
git push
```

Changes will appear on your live site within 1-2 minutes!

## Troubleshooting

- **404 Error**: Wait a few minutes for GitHub Pages to build
- **Styles not loading**: Check that all paths use `media/` not `../media/`
- **Images not showing**: Verify image paths are correct

## Need Help?

Check GitHub Pages documentation: https://docs.github.com/en/pages

