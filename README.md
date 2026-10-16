# MP Mokgotho Electrical – Invoice, Quotation & Inspection Letter Generator

A fast, mobile-first web app that runs entirely in the browser. No database, no server.

## Features
- Invoice, quotation and inspection letter in one app
- Automatic date and unique document numbers (INV / QUO / INS)
- Client details, add-more-rows items table, automatic totals, optional 15% VAT
- Letterhead, logo watermark, drawn digital signature and banking details
- Download PDF or Word, and upload a saved file to edit it again
- Email to a client (share the PDF from a phone, or open the email app)
- Installable on Android, works offline

## Structure
- `site/` the app (`index.html`, `manifest.webmanifest`, `sw.js`, `icons/`, `fonts/`, `jspdf.umd.min.js`)
- `.github/workflows/pages.yml` publishes `site/` to GitHub Pages on every push to `main`

## Run locally
Open `site/index.html` in a browser, or serve the folder:

    cd site && python3 -m http.server 8080

## Publish
1. Push to GitHub.
2. In the repository go to Settings > Pages and set Source to **GitHub Actions**.
3. The app is then live at `https://<your-username>.github.io/<repository-name>/`.

## Android app
Open the live address in Chrome on Android and choose **Install app**.
For an `.apk`, paste the live address into pwabuilder.com and package it for Android.

## Changing details
Company details, banking details and the footer text are near the top of the script in `site/index.html`
(`CO`, `BANK`, `CREDIT`) and in the letterhead and banking sections of the page.

---
Designed and powered by www.relohost.com, a division company of Morwa Nku Holdings.
