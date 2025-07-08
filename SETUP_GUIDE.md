# GitHub Pages Setup Guide

This guide will help you set up your GitHub Pages repository and deploy your personal website.

## Step 1: Create a New Repository on GitHub

1. Go to [GitHub](https://github.com) and sign in to your account
2. Click on the "+" icon in the top right corner and select "New repository"
3. Name your repository exactly as `stocastico96.github.io` (replace "stocastico96" with your GitHub username if different)
4. Make the repository public
5. Do not initialize it with a README, .gitignore, or license (we'll add these later)
6. Click "Create repository"

## Step 2: Initialize the Local Repository and Push to GitHub

Open a terminal and run the following commands:

```bash
# Navigate to your local repository directory
cd /Users/simone/Documents/GitHub/stocastico96.github.io

# Initialize a new Git repository
git init

# Add all files to the repository
git add .

# Commit the files
git commit -m "Initial commit"

# Add the remote GitHub repository
git remote add origin https://github.com/Stocastico96/stocastico96.github.io.git

# Push the files to GitHub
git push -u origin main
```

Note: If your default branch is named "master" instead of "main", use:

```bash
git push -u origin master
```

## Step 3: Configure GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" (tab with the gear icon)
3. Scroll down to the "GitHub Pages" section
4. Under "Source", select the branch you pushed to (main or master)
5. Click "Save"

GitHub will provide you with a link to your published site (usually https://stocastico96.github.io).

## Step 4: Add Your Profile Picture

1. Replace the placeholder image with your actual profile picture:
   - Name your image file `simone.png` or update the references in the HTML
   - Place it in the `assets` directory
   - Make sure it's properly sized (recommended: 200x200 pixels)

## Step 5: Verify Your Website

1. Wait a few minutes for GitHub Pages to build your site
2. Visit https://stocastico96.github.io to see your live website
3. Test all links and make sure everything works as expected

## Troubleshooting

- If your site doesn't appear, check the GitHub Pages section in your repository settings to see if there are any build errors
- Make sure your repository is named exactly `username.github.io`
- Ensure your files are in the root of the repository, not in a subdirectory

## Making Updates

Whenever you want to update your website:

1. Make changes to the files locally
2. Commit the changes:
   ```bash
   git add .
   git commit -m "Update website content"
   ```
3. Push to GitHub:
   ```bash
   git push origin main
   ```
4. Wait a few minutes for GitHub Pages to rebuild your site

## Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Custom Domain Setup](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- [GitHub Pages HTTPS Enforcement](https://docs.github.com/en/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https)
