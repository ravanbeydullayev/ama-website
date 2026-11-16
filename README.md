# AMA Website — GitHub Source Package

This package contains the currently approved/reviewed Azerbaijani source-page files for the AMA website, plus the Cookie Policy draft.

## Important status
- This is a source archive for starting the GitHub repository, **not yet a production-ready integrated website**.
- English versions and a site-wide AZ/EN language switch have **not yet been implemented**. They must be completed and tested before public deployment.
- The individual HTML files are preserved in `source-pages/`; they have not been merged into shared routing or a single deployable site.
- Cookie Policy V1 is a draft and is not marked approved.
- “İdarə Heyəti” is a homepage section (`#board`), not a separate page route. The Board sheet is a review artifact.
- Login, membership, dashboard, payment, email/OTP and admin functions may still be frontend prototypes. Backend and security work is required before production.

## Upload to GitHub
1. Create a new, separate repository named `ama-website` (do not use the SMF repository).
2. Extract this ZIP on your computer.
3. Upload the extracted `AMA-GitHub-Preparation` folder contents to the new repository, or use GitHub Desktop.
4. Do not connect the repository to the public domain/Cloudflare Pages for production until the integrated AZ/EN site has been completed and tested.

## Next development stage
1. Integrate the approved pages into a consistent site structure.
2. Produce the English version of every page and section.
3. Implement a persistent, site-wide AZ/EN language selector.
4. Test navigation, forms, links, consent behavior and responsive layouts in both languages.
5. Only then prepare the production deployment configuration.
