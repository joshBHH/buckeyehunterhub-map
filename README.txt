# Buckeye Hunter Hub – Leaflet (No Mapbox) Map

This package runs on GitHub Pages and embeds into Wix via an iframe. No Mapbox token required.

## Publish on GitHub Pages
1. Create a **public** repo (e.g., `buckeyehunterhub-map`).
2. Upload `index.html` to the **root** of the repo.
3. In the repo: **Settings → Pages → Source: Deploy from a branch → Branch: main / (root)** → Save.
4. Visit: `https://<yourusername>.github.io/<repository-name>/`

## Embed in Wix
Use an Embed HTML element with:
```html
<iframe src="https://<yourusername>.github.io/<repository-name>/" style="width:100%; height:600px; border:none;"></iframe>
```

## Features
- Draw markers, lines, polygons, rectangles
- Edit/Delete drawings
- Auto-saves to **localStorage** in the browser
- **Export / Import** GeoJSON
- Fullscreen toggle

## Notes
- Tiles are from OpenStreetMap. For high-traffic/production, consider a paid tile provider (MapTiler, Stadia Maps).
- localStorage saves per visitor/browser; for shared persistence, you'll need a small backend (can be added later).
