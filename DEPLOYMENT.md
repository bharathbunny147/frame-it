# 🚀 Deploying FRAME.IT (`@frame.it_b`)

This Next.js 16 (Turbopack) project is fully verified and pre-configured for zero-config production deployment on **Vercel**, **Netlify**, or any cloud provider.

---

### Option 1: Direct Deploy with Vercel CLI (Fastest — 1 Minute)

Open your terminal in this project directory:

```powershell
# 1. Ensure Node.js is on PATH (if not already)
$env:PATH = "C:\Program Files\nodejs;" + $env:PATH

# 2. Run Vercel CLI to link & deploy
npx vercel
```

When prompted:
- **Set up and deploy?** Press `y`
- **Which scope do you want to deploy to?** Choose your account / team
- **Link to existing project?** Press `n`
- **What's your project's name?** `frame-it` (or your preferred name)
- **In which directory is your code located?** `./` (press Enter)
- **Want to modify settings?** Press `n`

Once the preview URL is generated, deploy directly to **Production**:
```powershell
npx vercel --prod
```

Your live website will be live at `https://frame-it.vercel.app` (or your chosen project name)!

---

### Option 2: Deploy via GitHub / GitLab / Bitbucket (Automatic CI/CD)

1. Initialize Git and commit the project:
   ```bash
   git init
   git add .
   git commit -m "feat: FRAME.IT redesign and deployment setup"
   ```
2. Create a new repository on [GitHub](https://github.com/new) and push your code:
   ```bash
   git remote add origin https://github.com/<your-username>/frame-it.git
   git branch -M main
   git push -u origin main
   ```
3. Go to [Vercel New Project Import](https://vercel.com/new).
4. Select the `frame-it` repository and click **Deploy**.
5. Every time you push a new commit, Vercel will automatically build and publish updates!

---

### Verification Checklist Completed

- [x] Production build passes with 0 errors (`npm run build`)
- [x] Static pages pre-rendered (`/` and `/_not-found`)
- [x] Package renamed to `frame-it`
- [x] Added `vercel.json` framework configuration
- [x] Responsive images & unoptimized flag configured for any CDN
- [x] All assets (logo, male reelmaker photos, Instagram reels) verified
