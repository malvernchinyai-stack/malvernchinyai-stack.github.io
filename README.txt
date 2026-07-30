MARIMO SOLAR — Quotes & Receipts  (PWA / TWA package)
=====================================================

This folder turns your app into an installable Android app.

Files:
  index.html               <- your app (with PWA hooks added)
  manifest.json            <- app name, colours, icons
  sw.js                    <- makes it work offline after first load
  icon-192.png             <- app icon
  icon-512.png             <- app icon (large)
  icon-maskable-512.png    <- app icon (Android adaptive)

QUICK STEPS
-----------
1. Put ALL of these files in a free GitHub Pages site
   (repository named  yourusername.github.io ).
2. Your app goes live at  https://yourusername.github.io/
3. Go to https://www.pwabuilder.com  , paste that URL, and click Package
   for stores -> Android. Download the package.
4. Keep the signing.keystore file and its passwords SAFE — you need them
   for every future update.
5. To look fully native (no address bar): from the downloaded package,
   put assetlinks.json into a folder called  .well-known  in your repo, so
   it is live at  https://yourusername.github.io/.well-known/assetlinks.json
6. Install the .apk on your phones, or upload the .aab to Google Play.

UPDATING LATER
--------------
Change your app? Just re-upload the new index.html to GitHub AND bump the
version in sw.js (marimo-v1 -> marimo-v2). No need to rebuild the APK unless
you change the app name, icon, or package id.
