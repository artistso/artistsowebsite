# Artistso — initial website review & enhancement notes

**Review date:** 2026-11-07
**Status:** Initial repository review and static-site build completed; production domain not tested or changed.

## Scope and limits

The connected GitHub repository (`artistso/artistsowebsite`) contained only an initial `README.md` at the start of this task. It did not include the live site's source, deployment settings, CMS/theme, analytics, forms, or Muse integration. Consequently, this is not a forensic audit of the running website, and no claims are made about its existing speed, accessibility, search rankings, security, or integration behavior. The public site and DreamHost account were not accessed.

## What is in the build

- New responsive editorial landing page with clear paths to explore, collaborate, or make contact.
- Flexible desktop/mobile layout and compact navigation for smaller screens.
- Semantic landmarks, a skip link, descriptive labels, visible keyboard focus, Escape-to-close navigation, and reduced-motion handling.
- Search/share metadata, canonical URL, page title, and a custom SVG favicon.
- Lightweight static implementation with no framework, build dependency, database, or third-party tracking code.
- DreamHost-oriented deployment guidance and a pre-publish verification checklist in `README.md`.

## Decisions to confirm with Artistso

1. **Positioning:** The draft describes Artistso as a creative home/community for independent artists. Confirm whether that reflects the real offer, audience, geography, and brand tone.
2. **Contact:** Verify `hello@artistso.com` exists and is monitored. It appears in the navigation, calls to action, and contact section.
3. **Content:** Replace broad introductory copy with approved specifics. Add genuine artist profiles, examples, proof points, and photographs/illustrations once rights and permissions are clear.
4. **Muse:** The repository contains no integration code or setup notes. Confirm what “integrated with Muse” means (for example, a Muse site builder workflow, API, or external service), what pages/assets it owns, and which files must remain untouched.
5. **Hosting:** Identify the live document root, whether a CMS or rewrite rules are present, and whether staging/SFTP deployment is available before replacing anything.

## Pre-launch QA

- Back up production and validate on staging before changing the DreamHost document root.
- Verify the email address and all mailto links; check every CTA on desktop and mobile.
- Test current browsers, keyboard-only use, screen-reader landmarks, 200% zoom, contrast, and reduced-motion preference.
- Check mobile menu open/close, Escape behavior, focus visibility, and in-page anchor targets.
- Run HTML/CSS validation and a Lighthouse/PageSpeed pass; fix any issues found against the real deployed environment.
- Verify HTTPS, canonical URL, page title/description, favicon, Open Graph preview, and any needed `robots.txt`/sitemap.
- Confirm the Muse integration still works after staging deployment. Do not overwrite its assets, rewrite rules, or routes until ownership is clear.
- If analytics, embedded media, a mailing list, or a server-backed form is added later, document its data handling and required privacy notices.

## Recommended next iteration

Get the current site source or a production URL/screenshot and the precise Muse workflow, then review actual pages, content, mobile rendering, and integration boundaries. Agree on final positioning and brand assets, add real portfolio/artist content, and deploy through a backed-up staging-to-production change on DreamHost. This static draft intentionally has no fake artist listings, nonfunctional submission form, or fabricated testimonials.
