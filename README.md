# NoCo Home Co. — V6 staging site

A static, no-build website for GitHub + Cloudflare Pages. **This is a review prototype, not a live lead-collection service.**

## Deploy to GitHub and Cloudflare Pages

1. Create a **private** GitHub repository named `noco-home-co` (or use an existing approved repository).
2. Upload the contents of this archive, retaining the `public/` folder at repository root. Commit on `main`.
3. Cloudflare Dashboard → Workers & Pages → Create application → Pages → **Connect to Git** → choose that GitHub repository.
4. Framework preset: **None**. Build command: **leave blank**. Build output directory: **`public`**. Production branch: **`main`**.
5. Save and Deploy. Cloudflare will show a `*.pages.dev` URL. Check links, desktop, mobile and intake there.
6. Each subsequent commit to `main` deploys automatically. Preview branches can be used for safe review.

## Important

- The intake is a **simulation**, does not submit leads and should not be represented as ready to receive jobs.
- The site has noindex meta tags, `/robots.txt`, and `X-Robots-Tag` to discourage search indexing while staging. Do not treat `noindex` as access control. Set up Cloudflare Access if you need a private/password-protected review.
- Illustrative images are not photographs of actual NoCo staff or jobs.
- Do not remove staging protections until business identity, licensing, insurance, permitted service area, real staff and subcontractor credentials, customer contracts, privacy terms, accessible contact points and live lead handling are approved.
- This project is static HTML; do not choose a Next.js/Astro build preset.

## Files

- `public/index.html`: homepage
- `public/lets-get-it-fixed.html`: simulated intake
- `public/*-repair.html`, `public/exterior-repairs.html`: services
- `public/homeowner-guides.html`: AEO article index
- `public/_headers` and `public/robots.txt`: staging search restrictions
- `LAUNCH_GATES.md`: checklist for going live
