# Google Analytics Setup Guide

## What's Been Added

✅ Google Analytics 4 (GA4) tracking code on all pages
✅ Page view counter in footer (local browser tracking)
✅ Template ready for future articles

## Current Status

The tracking code is installed but **not yet active** because you need to:
1. Create a Google Analytics account
2. Set up a property for your website
3. Get your Measurement ID
4. Replace the placeholder in your code

## Step-by-Step Setup

### 1. Create Google Analytics Account
- Go to **https://analytics.google.com/**
- Click "Start measuring"
- Sign in with your Google account
- Create a new account (or use existing)

### 2. Create a Property
- Property name: `CloudDusk Blog` (or your choice)
- Reporting timezone: Your timezone
- Currency: USD (or your choice)
- Click "Create"

### 3. Create a Web Data Stream
- Platform: Web
- Website URL: `https://yourdomain.com` (your actual blog domain)
- Stream name: `CloudDusk Blog`
- Click "Create stream"

### 4. Get Your Measurement ID
- After creating the stream, you'll see your **Measurement ID**
- It looks like: `G-XXXXXXXXXX`
- Copy this ID

### 5. Update Your Files
Replace `G-XXXXXXXXXX` with your actual Measurement ID in:
- `index.html`
- `posts/2026-08-15-fabric-private-link.html`
- `ARTICLE_TEMPLATE.html`

**Find and replace this:**
```
G-XXXXXXXXXX
```

**With your actual ID (e.g.):**
```
G-AB12CD34EF
```

## Features

### Page View Counter in Footer
- Shows local page views for your browser (using localStorage)
- Each page tracks separately
- Resets when you clear browser data

**Note:** This is browser-only. Real analytics come from Google Analytics dashboard.

### Google Analytics Dashboard
Once set up, you can see:
- Total page views
- Unique visitors
- Traffic sources (search, direct, referral, etc.)
- Visitor behavior and flow
- Device/browser information
- Geographic data
- Much more!

Visit **https://analytics.google.com/** to view your dashboard.

## Verify It's Working

1. Update your Measurement ID in all files
2. Push changes to your live website
3. Visit your blog
4. Wait 24-48 hours for data to appear in Google Analytics dashboard
5. Check https://analytics.google.com/ to see your traffic

## For Future Articles

The `ARTICLE_TEMPLATE.html` already includes the tracking code with the placeholder. After you update the Measurement ID once, all new articles will automatically track when created from the template.

## Privacy Notice

You should add a privacy policy mentioning you use Google Analytics. This is especially important if you have international visitors.

Simple example to add to your site:
```
"This site uses Google Analytics to understand how visitors use the site."
```
