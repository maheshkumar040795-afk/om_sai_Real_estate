# Om Sai Real Estate — Go-Live Checklist (omsairealestates.co.in)

## 1. Upload to GitHub
Push ALL files in this folder to the repo root, including `CNAME` and `.nojekyll` (hidden file).

## 2. DNS (at your domain registrar)
| Type  | Host | Value |
|-------|------|-------|
| A     | @    | 185.199.108.153 |
| A     | @    | 185.199.109.153 |
| A     | @    | 185.199.110.153 |
| A     | @    | 185.199.111.153 |
| CNAME | www  | maheshkumar040795-afk.github.io |

Delete any default parking A/CNAME records first.

## 3. GitHub Pages
Settings → Pages → Custom domain: `omsairealestates.co.in` → Save → wait for DNS check → tick **Enforce HTTPS**.

## 4. Firebase (important — property listings load from Firebase)
Firebase Console → Authentication → Settings → **Authorized domains** → add
`omsairealestates.co.in` and `www.omsairealestates.co.in`.
Without this, anonymous sign-in / admin portal can fail on the new domain.

## 5. Google Search Console
1. Add property → URL prefix `https://omsairealestates.co.in/`
2. Choose "HTML tag", paste the tag into the commented line in `index.html` head, push, click Verify.
3. Sitemaps → submit `sitemap.xml`
4. URL Inspection → Request indexing for `/`, `/about.html`, `/contact.html`

## 6. After live — test
- https://omsairealestates.co.in/robots.txt
- https://omsairealestates.co.in/sitemap.xml
- https://omsairealestates.co.in/anything-wrong → branded 404 page
- Share the link on WhatsApp → preview card should show the logo
- Rich Results test: https://search.google.com/test/rich-results

## 7. Local SEO boost
Create/claim a **Google Business Profile** for Om Sai Real Estate (Madhavaram) and add the website link — this matters more than keywords for "real estate near me" searches.
