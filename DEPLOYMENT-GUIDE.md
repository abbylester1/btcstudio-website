# BTCstudio Website - Complete Deployment Guide

## 🚀 Deploy with GitHub + Netlify (Automatic Updates!)

This is the **BEST** method because:
- ✅ Free hosting forever
- ✅ Automatic deployments when you update
- ✅ Version control (track all changes)
- ✅ Easy to edit and update
- ✅ Professional workflow

---

## 📋 Step-by-Step Guide

### **Step 1: Create GitHub Account** (if you don't have one)
1. Go to: https://github.com
2. Click "Sign up"
3. Create account (use your email)
4. Verify your email

---

### **Step 2: Create New Repository**
1. Click the "+" icon in top-right → "New repository"
2. Fill in:
   - **Repository name:** `btcstudio-website`
   - **Description:** "BTCstudio - Bitcoin Development Studio Website"
   - **Public** ✅ (checked)
   - **Add README** ❌ (unchecked - we have one)
3. Click "Create repository"

---

### **Step 3: Upload Files to GitHub**

You have 4 files to upload:
- `index.html` (the website)
- `README.md` (documentation)
- `.gitignore` (Git configuration)
- `netlify.toml` (Netlify configuration)

**Method A: Via GitHub Website (Easy)**
1. On your new repository page, click "uploading an existing file"
2. Drag all 4 files into the upload area
3. Scroll down and click "Commit changes"

**Method B: Via Git Command Line (Advanced)**
```bash
# In your terminal/command prompt
cd /path/to/your/files
git init
git add .
git commit -m "Initial commit: BTCstudio website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/btcstudio-website.git
git push -u origin main
```

---

### **Step 4: Connect to Netlify**

1. Go to: https://www.netlify.com
2. Click "Sign up" → Choose "GitHub"
3. Authorize Netlify to access your GitHub
4. Click "Add new site" → "Import an existing project"
5. Choose "GitHub"
6. Find and select `btcstudio-website` repository
7. **Build settings:**
   - Build command: (leave empty)
   - Publish directory: `.` (just a dot)
8. Click "Deploy site"
9. Wait 30 seconds...
10. **Your site is LIVE!** 🎉

You'll get a URL like: `https://random-name-123456.netlify.app`

---

### **Step 5: Customize Your Netlify URL** (Optional)

1. In Netlify dashboard, click "Site settings"
2. Click "Change site name"
3. Enter: `btcstudio`
4. Your new URL: `https://btcstudio.netlify.app`

---

### **Step 6: Connect Custom Domain** (If you have one)

#### In Netlify:
1. Go to "Domain management"
2. Click "Add custom domain"
3. Enter your domain: `btcstudio.com` or `yourdomain.com`
4. Click "Verify"
5. Netlify will show DNS instructions

#### In Your Domain Registrar (GoDaddy, Namecheap, etc.):

**Option A: Using DNS Records**
```
Type: A
Name: @
Value: 75.2.60.5

Type: CNAME  
Name: www
Value: btcstudio.netlify.app
```

**Option B: Using Netlify DNS (Recommended)**
1. Netlify provides nameservers like:
   - `dns1.p01.nsone.net`
   - `dns2.p01.nsone.net`
   - `dns3.p01.nsone.net`
   - `dns4.p01.nsone.net`
2. Copy these nameservers
3. Go to your domain registrar
4. Find "Nameservers" or "DNS Settings"
5. Replace with Netlify's nameservers
6. Save
7. Wait 24-48 hours for DNS propagation

#### Enable HTTPS:
- Netlify automatically provides free SSL
- Once domain connects, go to "Domain management" → "HTTPS"
- Click "Verify DNS configuration"
- Click "Provision certificate"
- Wait ~1 minute
- Your site is now secure: `https://yourdomain.com` 🔒

---

## ✏️ How to Update Your Website

### Method 1: Edit on GitHub (Easy)
1. Go to your repository: `https://github.com/YOUR_USERNAME/btcstudio-website`
2. Click on `index.html`
3. Click the pencil icon (Edit)
4. Make your changes
5. Scroll down, click "Commit changes"
6. **Netlify automatically deploys in 30 seconds!** ✨

### Method 2: Edit Locally (Advanced)
1. Download the repository as ZIP
2. Edit `index.html` in any text editor (VS Code, Sublime, Notepad++)
3. Go back to GitHub
4. Upload the new `index.html`
5. Netlify auto-deploys!

### Method 3: Using Git (Professional)
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/btcstudio-website.git
cd btcstudio-website

# Make your edits to index.html

# Commit and push
git add index.html
git commit -m "Updated website content"
git push

# Netlify deploys automatically!
```

---

## 🎯 What You Get

✅ **Free hosting forever**  
✅ **Automatic HTTPS/SSL**  
✅ **Global CDN (super fast)**  
✅ **Automatic deployments**  
✅ **Version control**  
✅ **Easy rollback to previous versions**  
✅ **Custom domain support**  
✅ **Professional workflow**

---

## 📊 Monitoring & Analytics

### View Deployment Status:
- Go to Netlify dashboard → "Deploys"
- See all deployments and their status
- Click any deployment to see details

### Add Analytics (Optional):
1. In Netlify, go to "Analytics"
2. Enable analytics
3. See visitor stats, page views, etc.

---

## 🔧 Troubleshooting

### Site not updating?
1. Check Netlify "Deploys" tab
2. Make sure latest deploy is successful (green checkmark)
3. Clear browser cache (Ctrl+F5 or Cmd+Shift+R)

### Custom domain not working?
1. Wait 24-48 hours for DNS propagation
2. Check DNS settings in your registrar
3. Use https://www.whatsmydns.net to check propagation
4. Contact Netlify support (excellent free support!)

### Email form not working?
- The form uses `mailto:` which opens the user's email client
- For better form handling, consider:
  - Netlify Forms (free)
  - Formspree
  - EmailJS

---

## 📞 Support

- **Netlify Docs:** https://docs.netlify.com
- **Netlify Support:** https://www.netlify.com/support
- **GitHub Docs:** https://docs.github.com

---

## 🎓 Next Steps

1. ✅ Deploy to GitHub
2. ✅ Connect to Netlify
3. ✅ Customize URL
4. ⬜ Add custom domain
5. ⬜ Enable analytics
6. ⬜ Add more content
7. ⬜ Integrate real form backend

---

**Congratulations!** You now have a professional deployment workflow! 🚀

Every time you update the code on GitHub, Netlify automatically rebuilds and deploys your site. No manual uploads needed!
