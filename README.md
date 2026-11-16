# AMA Website — GitHub deployment package

This is a first integrated static-site package assembled from the 15 reviewed HTML source pages.

## Start here
- `index.html` — homepage (default Azerbaijani)
- `about.html`, `activities.html`, `projects.html`, `media.html`, `contact.html`
- `login.html`, `dashboard.html`
- `student-membership.html`, `professional-membership.html`, `corporate-membership.html`
- `terms.html`, `privacy.html`, `cookie-policy.html`
- `board-preview.html` is a review sheet only. The live Board navigation must point to `index.html#board`.

## Language support — important implementation note
A persistent AZ/EN switch has been added to each page. The English display currently uses Google's website-translation widget at runtime, with Azerbaijani retained as the source language. It requires an internet connection and a third-party Google translation script. This is a functional first-pass language layer, **not a reviewed, human-translated English content set**. For a fully controlled production launch, replace it with reviewed English translations stored in the site source and test every form, consent message, legal page, and dashboard label.

The language preference is stored in browser localStorage. Each page also has a matching Azerbaijani source copy and an `/en/` entry copy. English copies start in English mode.

## Important production limitations
- This package is static HTML. Authentication, password reset, member registration, payment, email, CV uploads, admin operations, and dashboard data are prototypes and need secure backend integration.
- Cookie consent UI is present on the homepage, but actual analytics/marketing scripts must be gated by consent before production.
- Cookie Policy is a draft and has not been approved as final legal text.
- Terms and Privacy drafts require legal review and confirmation against actual data processing.
- Review all navigation, external links, mobile layouts, and translation output before publishing.

## Deploy
Upload the contents of this folder to the root of the `ama-website` GitHub repository. For Cloudflare Pages, connect that repository and use the root directory `/`. No build command is required for this static package.
