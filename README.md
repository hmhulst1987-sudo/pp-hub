# pp-hub

Cloudflare Pages app. Production URL: **https://hub.pixelpiraterij.online**
Pages dev URL: https://pp-hub.pages.dev

## Stack
- Self-contained HTML (single `index.html`)
- Tailwind CSS via CDN
- Lexend font + Material Symbols Outlined
- Brand colors: `#705E4C` primary, `#FDFBF7` background

## Deploy
This repo serves as source of truth. To redeploy current state to Cloudflare Pages:

```bash
npx wrangler@latest pages deploy . --project-name=pp-hub --branch=main --commit-dirty=true
```

Set `CLOUDFLARE_API_TOKEN` env var first (Pages:Edit scope).

## Part of the PixelPiraterij app suite

Hub: [hub.pixelpiraterij.online](https://hub.pixelpiraterij.online) lists all apps and provides shared account.

Made by [Pixel Piraterij](https://pixelpiraterij.nl) 🏴‍☠️
