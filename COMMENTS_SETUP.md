# Comment System Setup Guide

## Overview
Your blog now has a comment system integrated into:
- ✅ Main page (index.html) - General feedback section
- ✅ All article pages - Questions/feedback per article
- ✅ Future articles - Template provided

## Email Configuration

All comments are sent to: **dhakumar82@gmail.com**

The form uses **Formspree** (https://formspree.io) to handle email submissions.

## How It Works

1. **User submits a comment** via the form
2. **Formspree receives and validates** the submission
3. **Email sent to dhakumar82@gmail.com** with the comment details
4. **User sees a success message**

## Current Setup

- Form ID: `mjbkozwb`
- Endpoint: `https://formspree.io/f/mjbkozwb`
- This ID is already configured in all forms

## For New Articles

Use the provided `ARTICLE_TEMPLATE.html` as a starting point for new articles. The template includes:
- Proper HTML structure
- Comment section with form
- Correct stylesheet references
- Formspree form already configured

## If You Need to Change the Email

1. Go to https://formspree.io
2. Sign up with your account
3. Create a new form with your email
4. Copy the form ID from the confirmation
5. Replace `mjbkozwb` with your new form ID in:
   - `index.html` (feedback form)
   - `posts/2026-08-15-fabric-private-link.html` (comment form)
   - `ARTICLE_TEMPLATE.html` (for future articles)

Change this line:
```html
<form class="comment-form" action="https://formspree.io/f/REPLACE_WITH_YOUR_FORM_ID" method="POST">
```

## Testing

To test the comment form:
1. Open any page with a comment form
2. Fill in name, email, and comment
3. Click submit
4. You should receive an email at dhakumar82@gmail.com

## Styling

All comment section styles are already included in `styles.css` and are responsive for mobile devices.
