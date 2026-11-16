# AMA Website — Deployment V2

This package consolidates the approved AMA page designs into a navigable static-site structure for Cloudflare Pages.

## Entry points
- Azerbaijani homepage: `index.html`
- English homepage: `en/home.html`

## Main pages
`about.html`, `activities.html`, `projects.html`, `media.html`, `contact.html`, `login.html`, `student-membership.html`, `professional-membership.html`, `corporate-membership.html`, `dashboard.html`, `terms.html`, `privacy.html`, `cookie-policy.html`.

## Navigation fixes
- Homepage navigation now opens the corresponding standalone pages.
- Board navigation returns to the Board section on the homepage (`index.html#board` / `en/home.html#board`), not a separate route.
- Membership navigation returns to the homepage membership section.
- Login and membership CTAs point to the matching pages.
- AZ/EN controls navigate between paired page paths.

## Translation status — important
This is a navigation and deployment-structure repair. The English copies have English metadata and phrase-level translations for shared interface labels and key headings, but long-form body copy and some detailed page content still require full editorial translation before the English site should be treated as production-complete. Do not represent all English page text as fully translated yet.

## Backend limitations
Membership payments, authentication, dashboard data, form submissions, CV uploads, and admin operations remain frontend prototypes until connected to secure backend services.

## Deploy
Upload the contents of this folder to the root of the `ama-website` GitHub repository. Keep Cloudflare Pages build command blank and output directory `.`.
