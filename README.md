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

## v6 visual matching
The reference screenshots were compared directly at the same 1179×2556 resolution.
The detail hero was shortened, logo/title/amount/date sizing was tightened, and the rewards
panel was compressed so the lower cards appear at the same vertical positions as the source.

Typography now uses Revolut's publicly served Aeonik Pro Medium URL for display text, with
Inter Tight / Inter fallbacks. Body/UI text remains Inter, matching published Revolut design
system evidence. No font files are bundled in this project.

The detail view also extends through the iOS home-indicator safe area instead of ending early.

## v7 scrolled detail content
The lower transaction detail sections were added from the user's original screenshot:
- Card / Visa
- Payment source / Personal RON
- Statement download
- Exclude from analytics
- Transport category
- Merchant total
- All 7 transactions
- Get help

The special blue card, Personal/R, download, transport, and gray chevron icons are local transparent PNGs
extracted from the user's supplied original screenshot. The merchant title bar appears automatically after scrolling.

## v8 statement viewer
The Kontoauszug row now opens a separate statement viewer page.
The white paper is based on the provided screenshot reference, preserved as a PNG background
with only the small 'Generiert am DD.MM.YYYY' date line replaced dynamically with today's date.
A centered watermark with the user's name appears in the dark top bar above the white paper.

## v9 Home Screen branding
- Web app name changed to `Revolut`
- Browser title changed to `Revolut`
- Apple touch icon / PWA icon changed to a Revolut-style app icon based on Revolut's official icon guidelines
- Added 32×32 and 64×64 favicon PNGs

The visible school-project/UI-simulation marking in the interface remains unchanged.


## v10 fixes
- Replaced the split-button `Y` with a PNG cropped from the original screenshot
- Replaced the reward icon with a PNG cropped from the original screenshot
- Made the `-3 lei` amount bolder
- Fixed the statement page so the white paper fits correctly on mobile instead of overflowing/cropping
