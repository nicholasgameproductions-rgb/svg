NicholasGPProxy customized static frontend

Changes:
- Disabled two original ad-network script injections, ad notice, and upsell triggers.
- Removed Google Analytics from index/study pages and SVG HTML wrappers.
- Replaced visible Lucide branding with NicholasGPProxy and updated the emblem.
- Disabled remote release-sync handler from 2cccok.js, so upstream release updates do not replace this custom frontend.

Deployment:
- Host the contents of svg-main/ as a static website on HTTPS.
- A working compatible proxy/server backend is still needed for live browsing, AI, accounts, and games.
- Clear existing service workers and site cache when replacing an older deployment.
- Ads and redirects from third-party websites opened inside the proxy are not universally removed by this frontend change.
- Precompiled assets were patched; there is no source tree or build setup in this ZIP.
- External backend/API branding and policies cannot be changed by patching this frontend.
