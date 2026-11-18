# Herman's Arcade

Landing page only. Game source code and game Git repositories are kept separately on the local computer. The browser games are deployed directly to Cloudflare Workers.

Public page: https://herman-vibecoding.github.io/

## Edit and publish

Edit `index.html` and the images in `screenshots/`, then commit and push `main`. GitHub Pages uses **Deploy from a branch → main → /(root)**. `.nojekyll` keeps this a plain static site. No build step is needed.

Local preview: `python3 -m http.server 8080`, then open http://localhost:8080.

## Hosting costs

Static assets on Cloudflare have free, unlimited requests. Each game fits the Free plan's 20,000-file and 25 MiB-per-file limits. Run from the Kura's online co-op also consumes Workers and Durable Objects daily quotas. Account-wide usage determines multiplayer capacity; solo play uses static assets.

See [Cloudflare static asset limits](https://developers.cloudflare.com/workers/static-assets/billing-and-limitations/) and [Durable Objects pricing](https://developers.cloudflare.com/durable-objects/platform/pricing/).
