# Chicken Cop website

Static site, no build step, no trackers, no third-party fonts or scripts (fonts are self-hosted from the game).

| URL | File | Used for |
|---|---|---|
| `/` | index.html | Marketing URL (App Store), website (Play), store buttons |
| `/privacy` | privacy.html | Privacy policy URL in both stores and in the game |
| `/terms` | terms.html | Terms of use (Apple EULA can stay standard; link this in the description) |
| `/support` | support.html | Support URL (App Store), restore purchases + refunds help |
| `/parents` | parents.html | Parents' guide (linked from listing and Grown-ups menu) |
| `/app-ads.txt` | app-ads.txt | AdMob verification through the store listing's developer website |
| 404 | 404.html | Custom 404 (both hosts pick it up automatically) |

Hosting: GitHub Pages from the `main` branch root (`.nojekyll` turns off Jekyll). Links and asset paths are relative, so the
site works both at `https://labailey.github.io/chickencop-site/` and on the custom domain. To use the custom domain, add it
under Settings > Pages (this creates a `CNAME` file) and point the DNS at GitHub Pages.
When the store links exist, swap the two "Coming soon" buttons in index.html for the official badges and links.
Update privacy.html in the same change as any game feature that sends something new off the device.
