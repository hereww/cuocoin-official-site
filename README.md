# CUOCOIN Official Site

Official website source for [www.cuocoin.com](https://www.cuocoin.com/), presenting the Cornerstone EVM network project.

## Website

The current landing page includes:

- Animated blockchain network background
- Chinese, English, Korean, and Japanese localization
- Remembered language preference
- Project vision, network layers, roadmap, and Genesis sections
- Cloudflare Workers deployment configuration

## Structure

- `dist/index.html` — production landing page
- `dist/favicon.svg` — website icon
- `cloudflare/worker.js` — Cloudflare Worker serving the static site
- `cloudflare/wrangler.jsonc` — Worker and custom-domain configuration

## Deploy

Authenticate Wrangler with the Cloudflare account that manages `cuocoin.com`, then run:

```bash
npx wrangler@latest deploy --config cloudflare/wrangler.jsonc
```

The Worker is configured for `www.cuocoin.com`.
