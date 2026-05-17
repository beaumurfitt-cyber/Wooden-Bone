# Wooden Bone Garden and Landscape Website

Astro static-first lead generation website for Netlify + Cloudflare.

## Run locally
- `npm install`
- `npm run dev`
- `npm run build`

## Deploy to Netlify
1. Connect repo in Netlify.
2. Build command: `npm run build`
3. Publish directory: `dist`
4. Enable Netlify Forms.

## Cloudflare custom domain
1. Add domain in Netlify.
2. In Cloudflare DNS, point CNAME/records per Netlify instructions.
3. Keep proxy enabled, SSL full/strict.

## Forms
- `/request-job` uses Netlify Forms (`data-netlify="true"`) with honeypot and file upload.
- Form redirects to `/thank-you`.

## Analytics placeholders
- `src/components/TrackingScript.astro` contains event hooks for GA4/GTM/Ads/Meta integrations.

## Add new suburbs
- Edit `src/data/site.ts` `suburbs` array.
- Dynamic routes generated at `/service-areas/[suburb]`.

## Add gallery items
- Edit `src/pages/before-after-gallery.astro` list and add images to `public/images/gallery/`.

## Add blog posts
- Add new page in `src/pages/blog/` and link from `src/pages/blog/index.astro`.

## Placeholders to replace before launch
- Phone, SMS, email, ABN, insurance/licensing, testimonials, logo, real project images.
