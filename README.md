# Resmokle — One‑Page Landing Site

This folder contains a ready‑to‑publish static site and a small media kit. It is designed for **GitHub Pages** + **custom domain**.

## What’s inside

- `index.html` — the landing page
- `assets/logo.svg` — simple logo
- `assets/hero.png` — hero banner
- `assets/social{1,2,3}.png` — square social posts (1080×1080)
- `assets/qr_resmokle.png` — QR pointing to https://resmokle.com
- `assets/favicon.png` — site icon
- `CNAME` — sets the domain to resmokle.com when deployed on GitHub Pages

## Quick publish (15–30 min)

1. Create a free GitHub account and verify email.
2. Click **New repository** → name it `resmokle` (Public).
3. Upload all files in this folder (including `CNAME`).
4. Go to **Settings → Pages** → set **Source** to `Deploy from a branch`, branch `main`, folder `/root` → **Save**.
5. After a minute, your site will be live at `https://<yourname>.github.io/resmokle/` and also at `https://resmokle.com` after DNS (step below).

### Connect your domain (GoDaddy → GitHub Pages)

1. In this repo, ensure there’s a file named `CNAME` (already included) that contains `resmokle.com` (exactly).
2. In **GoDaddy DNS**, add two records:
   - Type `A` → Name `@` → Value `185.199.108.153` (repeat for `185.199.109.153`, `185.199.110.153`, `185.199.111.153` — four A records total).
   - Type `CNAME` → Name `www` → Value `<yourname>.github.io`.
3. Wait for DNS to propagate (often 5–20 minutes). Refresh GitHub Pages settings until it shows a green check next to **Custom domain**.

### Enable the Forum (GitHub Discussions)

1. Repo → **Settings → General → Features** → check **Discussions**.
2. Repo → **Discussions** → copy the URL and paste it into the “Open the Forum” link in `index.html` (search for `Open the Forum` placeholder).

### Add the Contact Form (Google Forms)

1. Go to **forms.new** (logged into resmokle@gmail.com).
2. Create a form named **Resmokle Contact & Materials Pledge** with fields:
   - Name (short answer), Email, City/ZIP, What items do you have? (checkboxes), Volume estimate (short), Notes (paragraph).
3. Click **Send → <> Embed HTML** → copy the `<iframe …>` code.
4. Open `index.html`, find the placeholder `<iframe>` under “Contact Form” and replace it with your embed code. Save and upload changes.

### Optional: Analytics

- Create a **GA4** property at analytics.google.com → copy your tag (G-XXXX) → paste into `index.html` where indicated.

## Editing and updating

- You can edit `index.html` right in GitHub (pencil icon), then **Commit changes**. Pages redeploys automatically.

## Social media kit

Use the PNGs in `/assets` for day‑one posts. Suggested first captions are in your project plan.
