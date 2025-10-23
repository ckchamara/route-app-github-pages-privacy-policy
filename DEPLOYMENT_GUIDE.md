# RouteBus Privacy Policy & Feedback Website - Deployment Guide

This guide walks you through deploying the RouteBus privacy policy and feedback website to GitHub Pages.

## Current Status

✅ **Local Repository**: Initialized and ready
✅ **Files Created**: 
- `index.html` - Privacy Policy Website
- `feedback.html` - Feedback Form Page
- `README.md` - Project Documentation
- `FORM_SETUP_GUIDE.md` - Form Configuration Guide
- `privacy-policy.md` - Source Content

✅ **Git Commits**: 2 commits ready to push

## Prerequisites

Before deploying, ensure you have:
1. A GitHub account (https://github.com)
2. Git installed on your computer
3. Basic familiarity with GitHub

## Step-by-Step Deployment

### Step 1: Create the GitHub Repository

1. Go to https://github.com/new
2. Fill in the repository details:
   - **Repository name**: `route-app-github-pages-privacy-policy`
   - **Description**: `Privacy Policy website for RouteBus Flutter application - deployed via GitHub Pages`
   - **Visibility**: Public
   - **Initialize this repository with**: Leave all unchecked (we already have files)
3. Click **Create repository**

### Step 2: Push Your Local Repository to GitHub

After creating the repository, run these commands in your terminal:

```powershell
# Navigate to your project directory
cd f:\route-app-github-pages-privacy-policy

# Add the remote repository
git remote add origin https://github.com/ckchamara/route-app-github-pages-privacy-policy.git

# Verify the remote was added
git remote -v

# Push to GitHub
git push -u origin main
```

**Note**: You may be prompted to authenticate with GitHub. Use your GitHub credentials or a personal access token.

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub: https://github.com/ckchamara/route-app-github-pages-privacy-policy
2. Click on **Settings** (gear icon in the top right)
3. In the left sidebar, click **Pages**
4. Under "Build and deployment":
   - **Source**: Select "Deploy from a branch"
   - **Branch**: Select `main` and `/root` folder
   - Click **Save**

### Step 4: Wait for Deployment

GitHub Pages will automatically build and deploy your site:
- Initial deployment: 30-60 seconds
- Subsequent updates: 10-30 seconds

You'll see a message: "Your site is live at: `https://ckchamara.github.io/route-app-github-pages-privacy-policy/`"

### Step 5: Verify the Deployment

1. Visit the live URL: https://ckchamara.github.io/route-app-github-pages-privacy-policy/
2. Check that:
   - ✅ Privacy policy page loads correctly
   - ✅ All sections are visible and formatted properly
   - ✅ "Send Feedback" button is visible in the footer
   - ✅ Feedback page link works
3. Click "Send Feedback" to visit the feedback form
4. Verify the feedback form:
   - ✅ Form loads correctly
   - ✅ All fields are visible
   - ✅ Navigation links work
   - ✅ Form validation works (try submitting empty form)

## Setting Up Form Submissions

The feedback form is ready to use but needs a form submission service configured.

### Quick Setup with Formspree (Recommended)

1. Go to https://formspree.io and sign up
2. Create a new form and get your Form ID
3. Edit `feedback.html` and replace `YOUR_FORMSPREE_ID` with your actual ID
4. Commit and push the change:
   ```powershell
   git add feedback.html
   git commit -m "Configure Formspree form ID"
   git push
   ```

See `FORM_SETUP_GUIDE.md` for detailed instructions on alternative services.

## Live URLs

Once deployed, your website will be accessible at:

- **Privacy Policy**: https://ckchamara.github.io/route-app-github-pages-privacy-policy/
- **Feedback Form**: https://ckchamara.github.io/route-app-github-pages-privacy-policy/feedback.html

## Making Updates

### To Update the Privacy Policy

1. Edit `privacy-policy.md` with new content
2. Update `index.html` to reflect the changes
3. Commit and push:
   ```powershell
   git add index.html privacy-policy.md
   git commit -m "Update privacy policy content"
   git push
   ```
4. Changes will be live within 30 seconds

### To Update the Feedback Form

1. Edit `feedback.html` as needed
2. Commit and push:
   ```powershell
   git add feedback.html
   git commit -m "Update feedback form"
   git push
   ```
3. Changes will be live within 30 seconds

## Troubleshooting

### Repository Not Found Error
- Verify you created the repository on GitHub
- Check that the repository name matches exactly
- Ensure you're using the correct GitHub username

### Authentication Failed
- Use a personal access token instead of password
- Generate one at: https://github.com/settings/tokens
- Use the token as your password when prompted

### Site Not Deploying
- Check GitHub Pages settings (Settings → Pages)
- Verify branch is set to `main`
- Check for build errors in Actions tab
- Wait 1-2 minutes for initial deployment

### Form Not Submitting
- Verify Formspree ID is configured correctly
- Check browser console for errors (F12 → Console)
- Ensure you've verified your email in Formspree

## Custom Domain (Optional)

To use a custom domain:

1. Go to Settings → Pages
2. Under "Custom domain", enter your domain
3. Update your domain's DNS settings (see GitHub instructions)
4. GitHub will automatically provision an SSL certificate

## Monitoring

### View Deployment Status
1. Go to your repository
2. Click **Actions** tab
3. See deployment history and logs

### View Form Submissions
1. Log in to Formspree (if using Formspree)
2. View all submissions in your dashboard
3. Export data as needed

## Security Best Practices

1. ✅ Keep your GitHub credentials secure
2. ✅ Use personal access tokens instead of passwords
3. ✅ Enable two-factor authentication on GitHub
4. ✅ Review form submissions regularly
5. ✅ Keep privacy policy up to date
6. ✅ Monitor for spam submissions

## Support & Resources

- **GitHub Pages Docs**: https://docs.github.com/en/pages
- **Formspree Docs**: https://formspree.io/help
- **Git Documentation**: https://git-scm.com/doc
- **RouteBus Support**: support@routebus.app

## Next Steps

1. ✅ Create GitHub repository
2. ✅ Push local repository to GitHub
3. ✅ Enable GitHub Pages
4. ✅ Verify deployment
5. ✅ Configure form submission service
6. ✅ Test all functionality
7. ✅ Share the live URL with your team

## Summary

Your RouteBus privacy policy and feedback website is now ready to deploy! Follow the steps above to get it live on GitHub Pages. The site will be automatically updated whenever you push changes to the `main` branch.

For questions or issues, refer to the documentation files or contact support@routebus.app.

