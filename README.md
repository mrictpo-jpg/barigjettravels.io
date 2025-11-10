
# BARIGJET Travel Services – Static Landing Page

This repo contains a simple static site that can be hosted **free** on GitHub Pages.
Using a **custom domain** like `BARIGJETtravelServices.com` requires buying that domain from a registrar.

## Quick Deploy (GitHub Pages)
1) Create a new public repo named `barigjettravelservices`.
2) Upload these files. Make sure **index.html** is in the repo root (not in a folder).
3) In **Settings → Pages**, set:
   - Source: **Deploy from a branch**
   - Branch: **main** (or `master`) / folder: **/** (root)
4) After it builds, your site will be live at `https://<your-username>.github.io/barigjettravelservices/`.

## Connect Your Custom Domain
1) Buy `BARIGJETtravelServices.com` from a registrar (e.g., Namecheap, Google Domains, Cloudflare).
2) In your repo, keep the provided `CNAME` file with the domain name exactly.
3) In your registrar DNS, create the following records:

### If using apex/root domain
A     @  185.199.108.153
A     @  185.199.109.153
A     @  185.199.110.153
A     @  185.199.111.153
AAAA  @  2606:50c0:8000::153
AAAA  @  2606:50c0:8001::153
AAAA  @  2606:50c0:8002::153
AAAA  @  2606:50c0:8003::153

### (Optional) If using `www` subdomain
CNAME  www  <your-username>.github.io.

4) Back in **Settings → Pages**, add your custom domain, click **Save**, and enable **Enforce HTTPS**.

## Replace Assets
- Swap `images/logo.png` with your logo.
- Replace `images/hero-bg.jpg` with your background photo.
- Update text in `index.html` as needed.
