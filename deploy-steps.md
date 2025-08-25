# 🚀 Deployment Steps for Updated Website

## ✅ Files Ready for Deployment:
- ✅ `index.html` - Main website with updated navigation
- ✅ `resume.html` - Professional resume page with LinkedIn integration
- ✅ `CNAME` - Custom domain configuration
- ✅ Git repository initialized and committed

## 📋 Next Steps to Deploy:

### **Option 1: GitHub Pages (Recommended)**

1. **Create GitHub Repository:**
   - Go to [GitHub.com](https://github.com)
   - Click "New repository"
   - Name it: `dineshmurthy-website`
   - Make it **Public**
   - Click "Create repository"

2. **Connect Local Repository to GitHub:**
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/dineshmurthy-website.git
   git branch -M main
   git push -u origin main
   ```
   *(Replace YOUR_USERNAME with your actual GitHub username)*

3. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Under "Source", select "Deploy from a branch"
   - Choose "main" branch and "/(root)" folder
   - Click "Save"

4. **Configure Custom Domain:**
   - In the same Pages settings, add: `www.dineshmurthy.com`
   - Check "Enforce HTTPS" (after SSL is provisioned)
   - Click "Save"

### **Option 2: Netlify (Alternative)**

1. **Go to [Netlify.com](https://netlify.com)**
2. **Sign up/Login**
3. **Drag and drop** the entire `dineshmurthy-website` folder
4. **Add custom domain:** `www.dineshmurthy.com`
5. **Update DNS** as instructed by Netlify

## 🔧 DNS Configuration (if not already done):

Make sure your domain registrar has these DNS records:

**A Records for Root Domain:**
- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

**CNAME Record for www:**
- Name: `www`
- Value: `yourusername.github.io` (for GitHub Pages)

## 🌐 After Deployment:

Your website will be available at:
- **Main site:** https://www.dineshmurthy.com
- **Resume page:** https://www.dineshmurthy.com/resume.html

## 📱 Features Deployed:
- ✅ Responsive navigation with all menu items
- ✅ Professional resume page with LinkedIn integration
- ✅ Custom domain configuration
- ✅ Modern, mobile-friendly design
- ✅ Smooth scrolling and animations

## ⏱️ Timeline:
- **GitHub Pages:** 5-10 minutes to deploy
- **DNS Propagation:** 1-48 hours (usually 1-2 hours)
- **SSL Certificate:** 24-48 hours after domain setup

## 🆘 Need Help?
If you encounter any issues:
1. Check the `deployment-guide.md` file for detailed instructions
2. Verify DNS records are correct
3. Wait for DNS propagation before testing
4. Try accessing with HTTP first, then HTTPS 