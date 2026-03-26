# HELM — helm.vet landing page

Static landing page for HELM. Single HTML file with all assets embedded.

## Deploy to Vercel

### Option 1 — Vercel CLI (fastest)
```bash
npm i -g vercel
vercel
```
Follow the prompts. On first deploy it will ask you to link to a project — choose "Create new project" and name it `helm-site`.

### Option 2 — GitHub → Vercel (recommended)

1. Push this repo to GitHub:
```bash
git init
git add .
git commit -m "Initial commit — HELM landing page"
git remote add origin https://github.com/YOUR_ORG/helm-site.git
git push -u origin main
```

2. Go to [vercel.com](https://vercel.com) → New Project → Import from GitHub
3. Select `helm-site`
4. Framework Preset: **Other**
5. Root Directory: `/` (leave as default)
6. Click **Deploy**

### Custom domain (helm.vet)
After first deploy:
1. Vercel Dashboard → Project → Settings → Domains
2. Add `helm.vet` and `www.helm.vet`
3. In Cloudflare DNS, Vercel will give you the CNAME/A records to add

## Files
- `index.html` — full landing page, all assets (image, fonts) self-contained
- `vercel.json` — Vercel routing config
