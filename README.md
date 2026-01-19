# FamBams - Vercel Deployment Guide

## Quick Start

### Option 1: Deploy via Vercel Website (Easiest)

1. **Go to Vercel**: https://vercel.com
2. **Sign up/Login** (can use GitHub, GitLab, or email)
3. **Click "Add New"** → **"Project"**
4. **Upload these files**:
   - index.html
   - vercel.json
5. **Deploy!** Vercel will automatically build and deploy

### Option 2: Deploy via Vercel CLI

1. **Install Vercel CLI**:
   ```bash
   npm install -g vercel
   ```

2. **Login to Vercel**:
   ```bash
   vercel login
   ```

3. **Navigate to your project folder** (where these files are)

4. **Deploy**:
   ```bash
   vercel
   ```

5. **Follow the prompts**:
   - Set up and deploy? **Y**
   - Which scope? (Choose your account)
   - Link to existing project? **N**
   - What's your project's name? **fambams**
   - In which directory is your code located? **.**
   - Want to modify settings? **N**

6. **Deploy to production**:
   ```bash
   vercel --prod
   ```

## Connecting Your Custom Domain (fambams.com)

1. **Go to your Vercel Dashboard**: https://vercel.com/dashboard
2. **Click on your FamBams project**
3. **Go to Settings** → **Domains**
4. **Add "fambams.com"**
5. **Follow Vercel's DNS instructions**:
   - Go to your domain registrar (where you bought fambams.com)
   - Add the DNS records Vercel provides
   - Usually an A record pointing to Vercel's IP
   - And a CNAME for www

6. **Wait for DNS propagation** (can take up to 48 hours, usually faster)

## Your Firebase Config is Already Set Up!

Your app already has the Firebase configuration embedded, so it will work immediately once deployed.

## Testing Your Deployment

Once deployed, Vercel will give you a URL like:
- `https://fambams.vercel.app` (or similar)
- Or your custom domain once DNS is set up

## Troubleshooting

**If the app doesn't load:**
- Check browser console for errors (F12 → Console tab)
- Verify Firebase project is active at https://console.firebase.google.com

**If domain doesn't connect:**
- DNS can take time to propagate
- Double-check DNS settings in your domain registrar
- Use https://www.whatsmydns.net to check propagation

## Next Steps After Deployment

1. Test login/signup functionality
2. Test creating kids and events
3. Test inviting family members
4. Share the link with your family!

## Need Help?

- Vercel Docs: https://vercel.com/docs
- Firebase Docs: https://firebase.google.com/docs
