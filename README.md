# RouteBus Privacy Policy Website

This repository contains the static website for the RouteBus privacy policy, deployed via GitHub Pages.

## Overview

This is a simple, clean, and mobile-responsive website that displays the privacy policy for the RouteBus Flutter application. The privacy policy is converted from Markdown to a professional HTML page with modern styling.

## Files

- **index.html** - The main privacy policy website (HTML with embedded CSS)
- **feedback.html** - The feedback form page for user submissions (HTML with embedded CSS and JavaScript)
- **privacy-policy.md** - The source Markdown file containing the privacy policy content
- **README.md** - This file

## Features

### Privacy Policy Page
- ✅ Clean, professional design with gradient header
- ✅ Fully responsive (mobile, tablet, desktop)
- ✅ Easy to read with proper typography and spacing
- ✅ Organized sections with clear navigation
- ✅ Accessible and SEO-friendly
- ✅ Fast loading (single HTML file, no external dependencies)

### Feedback Form Page
- ✅ Professional feedback form with validation
- ✅ Multiple feedback types (Bug Report, Feature Request, General Feedback, Complaint, Compliment)
- ✅ Real-time form validation with visual feedback
- ✅ Success/error message display
- ✅ Mobile-responsive design matching privacy policy
- ✅ Integrated form submission service (Formspree)
- ✅ Loading indicator during submission
- ✅ Navigation links between pages

## Deployment

This website is deployed using GitHub Pages. The site is automatically published from the `main` branch.

### Live URLs

- **Privacy Policy**: https://ckchamara.github.io/route-app-github-pages-privacy-policy/
- **Feedback Form**: https://ckchamara.github.io/route-app-github-pages-privacy-policy/feedback.html

## Form Submission Setup

The feedback form uses **Formspree** to handle form submissions. To enable form submissions:

### Step 1: Create a Formspree Account
1. Go to https://formspree.io
2. Sign up with your email
3. Create a new form project

### Step 2: Get Your Formspree ID
1. After creating a form, you'll receive a unique form ID (e.g., `f/abc123xyz`)
2. Copy this ID

### Step 3: Update the Feedback Form
1. Open `feedback.html`
2. Find the line: `const response = await fetch('https://formspree.io/f/YOUR_FORMSPREE_ID', {`
3. Replace `YOUR_FORMSPREE_ID` with your actual Formspree ID
4. Save and commit the changes

### Alternative Form Services
You can also use:
- **Google Forms** - Create a form and embed it
- **Netlify Forms** - If deployed on Netlify
- **Custom Backend** - Set up your own API endpoint
- **EmailJS** - Client-side email service

## How to Update

### Privacy Policy
1. Edit the `privacy-policy.md` file with the updated content
2. Update the `index.html` file to reflect the changes
3. Commit and push to the `main` branch
4. The changes will be automatically deployed to GitHub Pages

### Feedback Form
1. Edit the `feedback.html` file as needed
2. Ensure your Formspree ID is configured
3. Commit and push to the `main` branch
4. Changes will be live within seconds

## GitHub Pages Configuration

GitHub Pages is configured to:
- Deploy from the `main` branch
- Use the root directory as the source
- Automatically rebuild on every push

## Local Development

To view the website locally:
1. Open `index.html` or `feedback.html` in your web browser
2. Or use a local server:
   ```bash
   # Using Python 3
   python -m http.server 8000

   # Using Python 2
   python -m SimpleHTTPServer 8000

   # Using Node.js (with http-server)
   npx http-server
   ```

### Testing the Feedback Form Locally
- The form will show validation errors for invalid inputs
- To test actual submission, you need to configure Formspree ID
- Without Formspree ID, the form will show an error on submission (expected behavior)

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## License

© 2025 RouteBus. All rights reserved.

## Contact

For questions about the privacy policy, contact: privacy@routebus.app

