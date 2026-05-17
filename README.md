# Wooden Bone Garden and Landscape website

Static-first Astro lead-generation website for Netlify + Cloudflare.

## Local run
1. `npm install`
2. `npm run dev`
3. `npm run build`

## Netlify deployment
- Build command: `npm run build`
- Publish directory: `dist`
- Netlify Forms enabled for `/request-job`

## Cloudflare domain setup
1. Add domain in Netlify.
2. Add DNS records in Cloudflare as instructed by Netlify.
3. Use SSL Full (strict) and keep proxy enabled.

## Forms and guided quote flow
- `/request-job` is a multi-step Netlify form with honeypot and photo uploads.
- Events: `form_start`, `form_step_complete`, `photo_upload`, `form_submit`.
- Success redirect: `/thank-you`.

## Update contact details
- Edit `src/data/site.ts` for phone, SMS, email, ABN, insurance placeholders.

## Update seasonal campaign block
- Edit `seasonalCampaign` in `src/data/site.ts`.

## Add new suburbs
- Add suburb names to `suburbs` in `src/data/site.ts`.
- Update `getStaticPaths` list in `src/pages/service-areas/[suburb]/index.astro` if publishing a localised page.

## Add gallery items
- Add images into `public/images/gallery/`.
- Update `src/pages/before-after-gallery.astro` and homepage preview.

## Add blog posts
- Create a page in `src/pages/blog/`.
- Add link in `src/pages/blog/index.astro`.

## Placeholders to replace before launch
- Phone number, email, ABN, insurance/licensing, logo, John photo, testimonials, and real project images.
