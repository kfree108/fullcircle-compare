# Full Circle — comparison pages

fullcircleagency.com runs on **Framer**, which does not accept file deploys, so
these pages are hosted here on GitHub Pages instead of being stuck in staging.

**To put them live, pick one:**

1. **Subdomain (no risk to the main site).** Add a DNS CNAME
   `compare` → `kfree108.github.io`, then set the custom domain on this repo's
   Pages settings to `compare.fullcircleagency.com`.
   Confirm propagation on 8.8.8.8, 1.1.1.1 and 9.9.9.9 **before** setting the
   custom domain — attaching against stale DNS makes GitHub queue the certificate
   and silently give up. That cost 90 minutes on drppc.ai.

2. **Rebuild them inside Framer.** The content is in `compare/*/index.html` and
   the source docs are in `remktr-gtm/staging/bofu/fullcircle/*/meta.json`.

3. **Move fullcircleagency.com off Framer**, as drppc.ai was moved off Squarespace.

Until then the Pages URL serves everything: https://kfree108.github.io/fullcircle-compare/
