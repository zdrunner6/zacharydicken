# Deploying ZacharyDicken.Com

Your site is ready to go live at **zacharydicken.com**. Here's how to connect your domain.

---

## Option 1: Vercel (Recommended — Free, Fast)

1. Push your project to GitHub (or create a new repo)
2. Go to [vercel.com](https://vercel.com) and sign in with GitHub
3. Click **Add New Project** → import your repo
4. Vercel auto-detects static HTML — click **Deploy**
5. **Add your domain:**
   - Project Settings → Domains → Add `zacharydicken.com` and `www.zacharydicken.com`
   - Vercel will show you DNS records

### DNS Records (at your domain registrar)

Add these at GoDaddy, Namecheap, Cloudflare, or wherever you bought the domain:

| Type | Name | Value |
|------|------|-------|
| A | @ | `76.76.21.21` |
| CNAME | www | `cname.vercel-dns.com` |

---

## Option 2: Netlify (Also Free)

1. Push to GitHub
2. Go to [netlify.com](https://netlify.com) → **Add new site** → **Import an existing project**
3. Connect GitHub, select the repo, deploy
4. **Add domain:** Site settings → Domain management → Add custom domain → `zacharydicken.com`
5. Netlify will show the DNS records to add at your registrar

### DNS Records for Netlify

| Type | Name | Value |
|------|------|-------|
| A | @ | `75.2.60.5` |
| CNAME | www | `[your-site-name].netlify.app` |

---

## Option 3: GitHub Pages (Free)

1. Push project to a GitHub repo
2. Repo → Settings → Pages
3. Source: **Deploy from a branch**
4. Branch: `main`, folder: `/ (root)` → Save
5. Add custom domain: `zacharydicken.com` in the Pages settings
6. Add DNS records (GitHub will show them)

### DNS for GitHub Pages

| Type | Name | Value |
|------|------|-------|
| A | @ | `185.199.108.153` (and 3 other IPs) |
| CNAME | www | `[username].github.io` |

---

## Your Files

- `index.html` — Main site (served at zacharydicken.com)
- `zacharydicken.html` — Same content (keep for reference)
- Meta tags, canonical URL, and Open Graph are set for **https://zacharydicken.com**

## After DNS propagates (5 min – 48 hrs)

Visit **https://zacharydicken.com** — you should see your site live.
