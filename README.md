# Artistso website starter

A responsive, dependency-free static landing page for [artistso.com](https://artistso.com), prepared for standard Apache hosting such as DreamHost. The working repository contained only an initial README when reviewed; this site is a fresh, editable foundation—not a source-level modification of the live production site.

Source of truth: [github.com/artistso/artistsowebsite](https://github.com/artistso/artistsowebsite) (this work is on the `arena/7a5a96aa-artistsowebsite` branch).

## Contents

- `index.html` — semantic landing page, page metadata, and editable copy
- `styles.css` — responsive visual system, mobile navigation layout, and reduced-motion support
- `script.js` — accessible mobile navigation and dynamic copyright year
- `favicon.svg` — matching vector mark
- `robots.txt` and `sitemap.xml` — basic crawl directives and sitemap
- `SITE_REVIEW.md` — scope, review notes, pre-launch checklist, and follow-up recommendations

## Preview locally

Run any static HTTP server from this directory, for example:

```sh
python3 -m http.server 8000 --bind 0.0.0.0
```

Then open `http://localhost:8000` on the same machine. No build step, package manager, or server runtime is required.

## Deploy to DreamHost

1. In the DreamHost panel, confirm the domain's configured web directory (the domain's document root) and whether the current site uses a CMS, custom `.htaccess`, or Muse-managed assets.
2. Back up the current web root before changing anything. Download a copy or create a dated archive first.
3. Test on a staging domain/subdomain if available. Do not overwrite existing integrations, API routes, CMS files, or `.htaccess` rules without confirming their purpose.
4. Upload the four site files to the intended web root using DreamHost's file manager or SFTP. The root `index.html` is the entry point; keep filenames and paths unchanged.
5. Confirm HTTPS is enabled for the domain in DreamHost, then test the home page, navigation, email links, mobile layout, and browser console.
6. Keep the previous site backup until the new page and any Muse integration have been verified.

This repo does not contain DreamHost credentials, production configuration, current Muse integration code, or a deployment pipeline. No production deployment has been attempted. The email address in the draft (`hello@artistso.com`) and all public-facing positioning should be verified before publishing.

## Customize before launch

- Confirm the intended business model, audience, services, and brand voice. The current page uses a deliberately broad creative-community positioning as a starting point.
- Verify `hello@artistso.com` routes to a monitored inbox, or replace every occurrence with the correct contact address.
- Add real work, artist profiles, testimonials, social profiles, and a social-sharing image only when approved assets and permissions are available.
- Confirm the canonical URL and metadata if the preferred domain or URL structure differs.
- Add privacy/cookie disclosures only if analytics, embeds, or other tracking are introduced.
