# Continuum Reader — open-access self-hosting handoff

This private repository belongs to `cyberwavestudios`. Download **ContinuumReader-open-access-source-and-assets.zip** from [the handoff release](https://github.com/cyberwavestudios/Continuum-Reader/releases/tag/open-access-handoff-2026-10-05). The same complete ZIP is also stored in the main branch. Do not use GitHub’s automatic “Source code (zip)” archive, which contains only this README and the package ZIP.

The ZIP includes the frontend, API, all 18 comic pages, cover, and sampler PDF, plus `SELF-HOSTING.md`. This edition serves all pages without a password, purchase token, Stripe, or PostgreSQL. Payment and order routes are not mounted. Historical purchase records and all secrets remain outside GitHub.

Type-check and production builds passed. The rebuilt API served page 18 without a token (HTTP 200); checkout returned HTTP 404. Deploy the frontend and API behind HTTPS, then test every page and the PDF on the replacement server before changing DNS or cancelling Replit. The live Replit app was not changed.
