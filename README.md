# Judith Mwangi | Portfolio website

A static site, ready for Vercel. No build step and nothing to install.

## Deploy on Vercel (about 5 minutes)

**Option A: drag and drop (easiest)**
1. Unzip this folder.
2. Go to vercel.com, sign in, click **Add New > Project**.
3. Choose to deploy without Git (or install the Vercel CLI and run `vercel` inside this folder).
4. Name the project **judithmwangi** so the address becomes `https://judithmwangi.vercel.app`.

**Option B: GitHub (best for updates)**
1. Create a GitHub repository and upload everything in this folder.
2. In Vercel, click **Add New > Project**, import the repository and press **Deploy**.
3. Every change you push to GitHub goes live automatically.

Framework preset: **Other**. Build command: leave empty. Output directory: leave as the root.

If Vercel gives you a different address, or you buy your own domain, replace
`https://judithmwangi.vercel.app` in these files: `index.html`, `robots.txt`, `sitemap.xml`.

## Make the booking form email you (one time)

The booking form sends requests through FormSubmit, a free form-to-email service.
1. After the site is live, make one test booking yourself.
2. FormSubmit sends an **activation email** to your Gmail. Click the link in it.
3. From then on every booking arrives in your inbox as a neat table.

Until activation, and if a visitor's browser blocks the request, the form still works:
it shows WhatsApp and email buttons with the booking already written, plus a calendar invite.

## Get found on Google

1. Open Google Search Console, add your site address and verify it.
2. Submit `sitemap.xml` under **Sitemaps**.
3. Add the site link to your LinkedIn profile (Contact info and Featured), email signature
   and the KYPW, AYPW and KeSEBAE profiles that mention you. Links from these sites are
   what push you up the results for "engineer Kenya" style searches.

## Add photos for projects that do not have one yet

Projects without a photo show a gold blueprint drawing. To swap in a real photo:
1. Save the photo as WebP or JPG in `images/` (for example `images/honey-refinery.webp`), ideally 1200px wide.
2. In `index.html`, find that project's `<div class="bp" ...> ... </div>` block and replace it with:
   `<img src="/images/honey-refinery.webp" width="1200" height="750" loading="lazy" alt="Describe the photo">`

## Privacy

No ID, passport, date of birth, postal address, registration numbers or referee
contacts appear anywhere. Your email and WhatsApp number are assembled by JavaScript
in the browser, so simple scraping bots cannot read them from the page source.

## Files

- `index.html` page content and SEO tags
- `css/style.css` design and animations
- `js/main.js` interactions, digital twin demo, booking
- `images/` optimised photos
- `vercel.json` security headers and caching
- `404.html`, `robots.txt`, `sitemap.xml`, `site.webmanifest`, icons, `og-image.jpg` (link preview image)
