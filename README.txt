ATH OWAY PWA package

FILES
- index.html: traveler app with visible App Install button
- admin.html: admin panel
- manifest.json: install metadata
- sw.js: service worker for PWA/offline app shell
- images/: app icons

DEPLOYMENT
1. Upload the ENTIRE folder contents to the same folder on an HTTPS website (not file://).
2. Keep index.html, admin.html, manifest.json, sw.js, and images/ together.
3. Open the website in Android Chrome. Tap “App ထည့်သွင်းရန်” and confirm Install.
4. On iPhone/iPad, open the site in Safari, tap Share, then Add to Home Screen. iOS does not allow a website to force the native install prompt; the button shows these steps.

IMPORTANT
- A website cannot force an install dialog immediately on page load. Browsers require a user gesture and decide when native installation is eligible. This package shows a prominent install button at the top.
- Install requires HTTPS hosting (localhost is allowed for development).
- The service worker provides a basic cached app shell.
- Admin data still uses LocalStorage in this version; it is not synchronized across different devices until a cloud database/storage backend is configured.
