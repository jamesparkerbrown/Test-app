# Word Blocks — Mobile PWA Package

This folder is ready to host as a Progressive Web App (PWA).

## Included
- index.html — your Word Blocks app
- manifest.webmanifest — app name, install/display settings, icons
- sw.js — offline service worker
- icon-192.png
- icon-512.png
- icon-maskable-512.png
- apple-touch-icon.png
- favicon-32x32.png

## Important
A PWA must be served from HTTPS (or localhost) for installation and offline service workers to work.
Opening index.html directly from your phone's Downloads folder is not enough.

## Easiest phone-only route
1. Create a GitHub repository from your phone/browser.
2. Upload every file in this folder to the repository root.
3. Enable GitHub Pages for the repository.
4. Open the Pages address in Chrome on Android.
5. Use the in-app "Install Word Blocks" button when it appears, or Chrome's menu > Install app / Add to Home screen.
6. After the first successful load, Word Blocks will work offline.

## If you later want an APK
Once the PWA is hosted, you can use a PWA-to-Android packaging service such as PWABuilder to create an Android package.

## Updating the app
If you change app files later, update CACHE_NAME in sw.js from:
  word-blocks-v1
to:
  word-blocks-v2
(or another new value) so installed devices refresh their cached copy.
