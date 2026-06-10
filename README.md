# Purus Building Maintenance - Website

Single-page luxury website for Purus Building Maintenance (puruscanada.ca).
Built with HTML + Tailwind CSS (CDN). No build step required.

## Package Contents

| File | Purpose |
|---|---|
| index.html | Full website (self-contained, logos embedded) |
| 404.html | Branded not-found page (GitHub Pages serves this automatically) |
| favicon.png | Browser tab icon (64x64) |
| apple-touch-icon.png | iOS home screen icon (180x180) |
| robots.txt | Crawler permissions + sitemap pointer |
| sitemap.xml | XML sitemap for Google Search Console |
| .nojekyll | Disables Jekyll processing on GitHub Pages |

## Deploy to GitHub Pages

1. Create a repo (e.g. `purus`) under the officialrevmedia account
2. Upload ALL files in this folder to the repo root
3. Settings > Pages > Source: Deploy from branch > main > / (root) > Save
4. Site goes live at: https://officialrevmedia.github.io/purus/

## Connecting the custom domain (when ready)

1. Settings > Pages > Custom domain: enter `www.puruscanada.ca` (this creates a CNAME file)
2. At the DNS provider, point: CNAME `www` -> `officialrevmedia.github.io`
3. Apex A records for puruscanada.ca: 185.199.108.153 / .109. / .110. / .111.153
4. Enable "Enforce HTTPS" once the certificate is issued
5. The canonical URL, sitemap and robots already reference https://www.puruscanada.ca/

## Activate the quote form (one-time, important)

The form posts directly to info@puruscanada.ca via FormSubmit:
1. After deploying, submit the form once with test data
2. FormSubmit emails a confirmation link to info@puruscanada.ca
3. Click "Activate" in that email. All future submissions then arrive in the inbox
4. If a send ever fails, the site automatically falls back to opening the visitor's email client

## Post-launch SEO checklist

- [ ] Verify the domain in Google Search Console and submit sitemap.xml
- [ ] Create / claim the Google Business Profile (91 Skyway Avenue, Suite 207, Toronto)
- [ ] Verify in Bing Webmaster Tools (imports from GSC in one click)
- [ ] Confirm LocalBusiness rich results: https://search.google.com/test/rich-results
