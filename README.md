# Spica Technologies Website

## What's in this folder
- `index.html` — Your complete website (photos embedded, ready to go)

## How to deploy (put it live on the internet)

### Option A: Vercel (recommended — free, 5 minutes)

1. Go to **vercel.com** and create a free account
2. Click **"Add New Project"**
3. Click **"Upload"** (no GitHub needed)
4. Drag and drop this entire folder into the upload area
5. Click **Deploy**
6. Your site is live at `spica-technologies.vercel.app`

To connect your custom domain (spicatech.com):
- In Vercel dashboard: **Settings → Domains → Add**
- Type `spicatech.com`
- Vercel gives you DNS records — paste them into your domain registrar (Cloudflare/Namecheap)
- Wait 5–30 minutes. Done.

### Option B: Cloudflare Pages (also free)

1. Go to **dash.cloudflare.com** → Pages → Create a project
2. Click **"Upload assets"**
3. Drag and drop this folder
4. Click **Deploy**
5. If your domain is on Cloudflare, it auto-connects

### Option C: Open in VS Code and deploy from there

1. Open VS Code
2. File → Open Folder → select this folder
3. You'll see `index.html` in the file list
4. To preview locally: right-click `index.html` → "Open with Live Server" (install the Live Server extension first)
5. To deploy to Vercel from VS Code terminal (bottom panel), type:

```
npm install -g vercel
vercel
```

6. Follow the prompts. It will ask you to log in and confirm. Then it's live.

## Making changes

Edit `index.html` in VS Code. All photos are embedded in the file as base64 data — no external dependencies.

To swap the leadership placeholder photo with your real photo:
1. Find the `👤` emoji in the HTML (search for it)
2. Replace the placeholder `<div>` with: `<img src="your-photo.jpg" style="width:100%;height:100%;object-fit:cover">`
3. Put your photo file in the same folder as `index.html`
