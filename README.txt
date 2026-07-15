STILLARIUM - INSTALL GUIDE
===========================

WHAT THIS IS
A self-contained web app. No database, no accounts, no dependencies.
All progress is saved in the phone's own browser storage.

UPLOAD TO HOSTINGER
1. Log in to hPanel and open File Manager for easttowestmedia.co.uk
2. Inside public_html, create a folder called: stillarium
3. Upload ALL of these files into that folder:
   index.html, app.js, sw.js, manifest.json, icon-192.png, icon-512.png
4. Visit https://easttowestmedia.co.uk/stillarium/ to check it loads
   (HTTPS is required for install and offline mode - Hostinger has this on by default)

INSTALL ON YOUR PHONE
iPhone:  open the URL in Safari > Share button > Add to Home Screen
Android: open the URL in Chrome > menu (three dots) > Install app

NOTES
- Works offline after the first visit (service worker caches everything)
- Progress lives on the device. Clearing the browser's site data wipes it,
  and it does not sync between devices
- To ship an update later: replace app.js (and bump "stillarium-v1" to
  "stillarium-v2" in sw.js so phones pick up the new version)
