# RouteBus Feedback Form Setup Guide

This guide explains how to configure the feedback form to handle submissions. The form is currently configured to use **Formspree**, but you can use alternative services as well.

## Quick Start with Formspree (Recommended)

Formspree is the easiest option for static sites. It's free, requires no backend, and handles email notifications automatically.

### Step 1: Create a Formspree Account
1. Visit https://formspree.io
2. Click "Sign Up" and create an account with your email
3. Verify your email address

### Step 2: Create a New Form
1. After logging in, click "New Form"
2. Give it a name: `RouteBus Feedback`
3. Set the email address where you want to receive submissions
4. Click "Create"

### Step 3: Get Your Form ID
1. You'll see a form ID like: `f/abc123xyz456`
2. Copy this ID (the part after `f/`)

### Step 4: Update feedback.html
1. Open `feedback.html` in a text editor
2. Find this line (around line 280):
   ```javascript
   const response = await fetch('https://formspree.io/f/YOUR_FORMSPREE_ID', {
   ```
3. Replace `YOUR_FORMSPREE_ID` with your actual ID
4. Save the file

### Step 5: Test the Form
1. Open `feedback.html` in your browser
2. Fill out the form and click "Send Feedback"
3. You should receive an email confirmation
4. Check your Formspree dashboard to see the submission

## Alternative Form Services

### Option 1: Google Forms (Free, No Setup Required)

**Pros:**
- Completely free
- No account needed
- Responses stored in Google Sheets
- Easy to analyze data

**Cons:**
- Less customizable
- Redirects to Google Forms page

**Setup:**
1. Create a Google Form at https://forms.google.com
2. Add fields matching our form (Name, Email, Feedback Type, Subject, Message)
3. Get the form's action URL
4. Update the form's `action` attribute in `feedback.html`

### Option 2: Netlify Forms (If Deployed on Netlify)

**Pros:**
- Integrated with Netlify deployment
- Free tier available
- Spam filtering included

**Cons:**
- Only works if deployed on Netlify
- Limited free submissions

**Setup:**
1. Deploy the site to Netlify
2. Add `netlify` attribute to the form: `<form netlify>`
3. Submissions appear in Netlify dashboard

### Option 3: EmailJS (Client-Side Email)

**Pros:**
- No backend required
- Sends emails directly
- Free tier available

**Cons:**
- Requires API key in frontend (less secure)
- Limited free emails per month

**Setup:**
1. Sign up at https://www.emailjs.com
2. Create an email service
3. Get your Service ID and Template ID
4. Update the JavaScript in `feedback.html` to use EmailJS

### Option 4: Custom Backend API

**Pros:**
- Full control
- Can integrate with your existing backend
- Most secure option

**Cons:**
- Requires backend development
- More complex setup

**Setup:**
1. Create an API endpoint on your server
2. Update the fetch URL in `feedback.html` to point to your endpoint
3. Handle form data and send emails from your backend

Example:
```javascript
const response = await fetch('https://your-api.com/api/feedback', {
    method: 'POST',
    headers: {
        'Content-Type': 'application/json',
    },
    body: JSON.stringify(data)
});
```

## Form Data Structure

The form sends the following data:

```json
{
    "name": "User's Name",
    "email": "user@example.com",
    "feedbackType": "bug-report|feature-request|general-feedback|complaint|compliment",
    "subject": "Brief subject",
    "message": "Detailed message",
    "timestamp": "2025-10-23T12:34:56.789Z",
    "userAgent": "Browser information"
}
```

## Email Notification Template

When using Formspree, you can customize the email template:

1. Go to your Formspree dashboard
2. Click on your form
3. Go to "Settings" → "Email Notifications"
4. Customize the email template to include:
   - Feedback Type
   - Subject
   - Message
   - User's contact information

## Troubleshooting

### Form Submission Shows Error
- Check that your Formspree ID is correct
- Verify you've verified your email in Formspree
- Check browser console for error messages (F12 → Console)

### Not Receiving Emails
- Check spam/junk folder
- Verify email address in Formspree settings
- Check Formspree dashboard for submission records

### CORS Errors
- This is normal for Formspree (it handles CORS)
- If using custom backend, ensure CORS headers are set

## Security Considerations

1. **Never expose sensitive API keys** in frontend code
2. **Validate all inputs** on the backend
3. **Implement rate limiting** to prevent spam
4. **Use HTTPS** for all submissions
5. **Store data securely** and comply with privacy regulations

## Monitoring Submissions

### With Formspree
1. Log in to https://formspree.io
2. View all submissions in your dashboard
3. Export data as CSV
4. Set up email notifications for new submissions

### With Custom Backend
1. Store submissions in your database
2. Create an admin dashboard to view submissions
3. Implement analytics and reporting

## Next Steps

1. Choose your preferred form service
2. Follow the setup instructions above
3. Test the form thoroughly
4. Deploy to GitHub Pages
5. Monitor submissions and respond to feedback

## Support

For issues with:
- **Formspree**: Visit https://formspree.io/help
- **Google Forms**: Visit https://support.google.com/forms
- **Netlify Forms**: Visit https://docs.netlify.com/forms/overview
- **EmailJS**: Visit https://www.emailjs.com/docs

For RouteBus feedback form issues, contact: support@routebus.app

