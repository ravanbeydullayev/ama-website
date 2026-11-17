# AMA Website Deployment V4

This package updates the V3 static site routing and navigation.

## Fixes included
- Privacy Policy, Terms of Use and Cookie Policy links now point to their dedicated pages (including English routes).
- Membership calls-to-action on both homepages now open the matching Student, Professional or Corporate membership application page rather than the login page.
- Language toggles now switch to the matching AZ/EN page pair and preserve the current section route.
- English pages have an initial visible-copy translation pass; review all wording before production publication.
- Separate Board page remains available at `/board.html` and `/en/board.html`.

## Deploy
Upload the contents of this folder to the root of the `ama-website` GitHub repository, replacing same-named files. Cloudflare Pages is configured for automatic deployment from `main`.

Note: authentication, payment processing, member approval, and application persistence still require backend integration.
