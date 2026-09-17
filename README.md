# Finance UI Demo — School Project

GitHub Pages / iPhone standalone web-app mockup.

## Merchant logos
The merchant identities were checked against current online sources:
- STB București: Wikimedia Commons entry for Societatea de Transport București
- Metrorex: Wikimedia Commons Metrorex logo entry
- Mega Image: official Mega Image careers site logo

The local PNG assets in this school-project package are matched to the merchant-avatar presentation visible in the supplied reference screenshots.

## Dynamic time
`PAYMENT_AGE_MINUTES = 12`

The latest STB payment is generated at the browser's current local time minus 12 minutes.
All other transactions in that same day are generated earlier than it.
The transaction details page reuses the exact same generated payment time.

## Publish
Upload all files to your GitHub repository root, then:
Settings → Pages → Deploy from a branch → main → /(root).

On iPhone:
Safari → Share → Add to Home Screen → Open as Web App.

## Typography update
Public design-system analyses consistently identify Aeonik Pro for Revolut display typography and Inter for body/UI.
Aeonik Pro is proprietary, so this package does not redistribute it. The mockup loads Inter from Google Fonts and
uses tuned weights/letter-spacing to approximate the app UI closely without bundling proprietary font files.

## Metrorex
`metrorex.png` was redrawn from the official Metrorex logo geometry referenced on Wikimedia Commons, which identifies
Metrorex as the author/source of the logo.
