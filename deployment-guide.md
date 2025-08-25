# Deployment Instructions for www.dineshmurthy.com

## Option 1: Using GitHub Pages (Recommended)

1. **Create a GitHub Repository:**
   - Go to GitHub.com and create a new repository named `dineshmurthy-website`
   - Upload the `index.html` file to the repository

2. **Enable GitHub Pages:**
   - Go to repository Settings > Pages
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click "Save"

3. **Configure Custom Domain:**
   - In the same Pages settings, add `www.dineshmurthy.com` as custom domain
   - Create a CNAME file in your repository with content: `www.dineshmurthy.com`

4. **Update DNS Records:**
   - Go to your domain registrar (where you bought dineshmurthy.com)
   - Add these DNS records:
     - Type: CNAME, Name: www, Value: yourusername.github.io
     - Type: A, Name: @, Value: 185.199.108.153
     - Type: A, Name: @, Value: 185.199.109.153
     - Type: A, Name: @, Value: 185.199.110.153
     - Type: A, Name: @, Value: 185.199.111.153

## Option 2: Using Netlify

1. **Deploy to Netlify:**
   - Go to netlify.com and sign up/login
   - Drag and drop the `index.html` file to deploy
   - Or connect your GitHub repository

2. **Configure Custom Domain:**
   - Go to Site settings > Domain management
   - Add custom domain: `www.dineshmurthy.com`
   - Update DNS records as instructed by Netlify

## Option 3: Using Vercel

1. **Deploy to Vercel:**
   - Go to vercel.com and sign up/login
   - Import your GitHub repository or upload files
   - Deploy automatically

2. **Configure Custom Domain:**
   - Go to Project settings > Domains
   - Add `www.dineshmurthy.com`
   - Update DNS records as instructed

## Option 4: Traditional Web Hosting

1. **Upload via FTP:**
   - Use an FTP client (FileZilla, WinSCP)
   - Upload `index.html` to your web server's public_html or www folder
   - Ensure the file is named `index.html` (default homepage)

## File Structure
```
/
├── index.html          # Main website file
└── deployment-guide.md # This deployment guide
```

## Testing
After deployment, visit:
- http://www.dineshmurthy.com
- https://www.dineshmurthy.com (if SSL is configured)

## Features of the Website
- ✅ Responsive design (mobile-friendly)
- ✅ Modern gradient background
- ✅ Smooth scrolling navigation
- ✅ Interactive hover effects
- ✅ All requested menu items: Me, Products, Solutions, Games, Help
- ✅ Professional styling with CSS animations
- ✅ SEO-friendly structure

## Next Steps
1. Choose your preferred hosting method
2. Follow the deployment instructions
3. Test the website on different devices
4. Consider adding more content to each section
5. Set up analytics (Google Analytics, etc.)
6. Configure SSL certificate for HTTPS 