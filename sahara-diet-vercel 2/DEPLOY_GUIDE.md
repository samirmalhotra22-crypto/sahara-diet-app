# SAHARA Diet App — Vercel Deployment Guide

## What you need
- Free GitHub account: github.com
- Free Vercel account: vercel.com  
- Free Anthropic account + API key: console.anthropic.com

---

## Step 1 — Get your Anthropic API Key (2 min)

1. Go to **console.anthropic.com** and sign in (or create free account)
2. Click **"API Keys"** in the left menu
3. Click **"Create Key"** → give it a name → click **"Create Key"**
4. **Copy the key** (starts with `sk-ant-`) — save it somewhere, you'll need it in Step 3

---

## Step 2 — Upload to GitHub (3 min)

1. Go to **github.com** → sign in
2. Click the **"+"** icon top right → **"New repository"**
3. Name it: `sahara-diet-app`
4. Keep it **Public** → click **"Create repository"**
5. Click **"uploading an existing file"** link
6. **Drag and drop the entire `sahara-diet-vercel` folder contents:**
   - `api/analyze.js`
   - `public/index.html`
   - `vercel.json`
   - `package.json`
7. Click **"Commit changes"**

---

## Step 3 — Deploy on Vercel (2 min)

1. Go to **vercel.com** → sign in with GitHub
2. Click **"Add New Project"**
3. Find and click **"sahara-diet-app"** → click **"Import"**
4. Before clicking Deploy, click **"Environment Variables"**
5. Add this variable:
   - **Name:** `ANTHROPIC_API_KEY`
   - **Value:** paste your `sk-ant-...` key here
6. Click **"Add"** → then click **"Deploy"**
7. Wait ~30 seconds → your app is live! ✅

---

## Your app URL

Vercel gives you a URL like:
**`https://sahara-diet-app.vercel.app`**

Share this with anyone — photo scanning works automatically, no API key needed by users.

---

## Add to iPhone Home Screen

1. Open the URL in **Safari**
2. Tap the **Share button** (box with arrow at bottom)
3. Tap **"Add to Home Screen"**
4. Tap **"Add"**

It now looks and works like a native app on your phone! 📱

---

## Updating the app later

Just edit files in GitHub → Vercel auto-redeploys in ~30 seconds.

---

## Cost

- GitHub: **Free**
- Vercel: **Free** (up to 100GB bandwidth/month)
- Anthropic API: **~$0.003 per photo scan** (very cheap — 1000 scans ≈ $3)
