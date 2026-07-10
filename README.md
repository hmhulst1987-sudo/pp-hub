# pp-hub

Live public hub for PixelPiraterij. Production URL: **https://hub.pixelpiraterij.online**

## Stack
- Static `index.html`
- Generated `catalog.json` from `shared-product`
- Hosted on `pixelpiraterij-vps`
- Served from `/srv/pixelpiraterij-hub` behind Traefik

## Deploy
The public files in this folder are updated from the Android/shared product layer and deployed to the live VPS.

Build and deploy from:

```bash
C:\Users\Gebruiker\AndroidStudioProjects\PixelPiraterijAPPS
```

Commands:

```bash
node shared-product/scripts/build-all.mjs
node shared-product/scripts/deploy-hub.mjs
```

## Role in the PixelPiraterij stack

- `pixelpiraterij.nl` = commercial front door
- `pixelpiraterij.online` = engine / showroom / route proof
- `hub.pixelpiraterij.online` = app gallery / web suite / distribution layer

This repository is the public hub source of truth.

## Part of the PixelPiraterij app suite

Hub: [hub.pixelpiraterij.online](https://hub.pixelpiraterij.online) lists all apps and forms the canonical suite layer for web distribution.

Made by [Pixel Piraterij](https://pixelpiraterij.nl)
