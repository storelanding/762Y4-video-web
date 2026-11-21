# Video — website

Static website (no build step) for the **Video** Android app on Google Play.

| File | Purpose |
| --- | --- |
| `index.html` | App landing page |
| `policies.html` | Privacy Policy |
| `terms.html` | Terms of Use |
| `app-ads.txt` | Ads seller declaration |
| `404.html` | Not found page |
| `assets/` | CSS, icon and screenshots |
| `site.json` | Metadata used to generate the site |

## Deploy

**Cloudflare Pages:** Workers & Pages → Create → Pages → Connect to Git → choose this repo. Framework preset **None**, build command empty, output directory `/`. Add your domain under Custom domains.

**Vercel:** Add New → Project → import this repo. Framework **Other**, no build command, output directory `.`. Add your domain under Settings → Domains.

## After deploying

- `app-ads.txt` must be reachable at `https://<your-domain>/app-ads.txt`, and that domain must match the developer website declared on Google Play.
- Privacy Policy URL for the store listing: `https://<your-domain>/policies.html`.
