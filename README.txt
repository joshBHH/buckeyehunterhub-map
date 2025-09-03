Buckeye Hunter Hub — Deploy Bundle (GitHub Pages)
================================================

This bundle includes the PWA pieces. Add these files **next to your existing index.html**.

Files
-----
- manifest.webmanifest
- sw.js
- icons/icon-192.png
- icons/icon-512.png
- icons/icon-512-maskable.png (maskable icon for Android install prompt)
- favicon.ico (optional)

Install
-------
1) Place everything in the same folder as your index.html (create the icons/ folder).
2) In <head> of index.html:
   <link rel="manifest" href="./manifest.webmanifest">
   <meta name="theme-color" content="#0b1a0f">
   <link rel="icon" href="./favicon.ico">
3) Near </body> of index.html:
   <script>
     if ('serviceWorker' in navigator) {
       navigator.serviceWorker.register('./sw.js');
     }
   </script>
4) Commit & push. Visit your site on mobile to "Add to Home Screen".

Notes
-----
- Ensure your JS uses a real MapTiler key (replace YOUR_MAPTILER_KEY).
- The Ohio public lands file is optional; if you reference it, put it next to index.html.
