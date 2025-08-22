# Buckeye Hunter Hub – Hunting Map

This repository hosts the interactive hunting map for [Buckeye Hunter Hub](https://www.buckeyehunterhub.com), built with **Leaflet.js** and **Leaflet.draw**.

## Features
- 🗺️ **Interactive Map** centered on Ohio (OpenStreetMap basemap)
- ✏️ **Drawing Tools** – add points, lines, and polygons
- 💾 **Local Persistence** – drawings are saved to browser localStorage
- 📂 **Import / Export** drawings as GeoJSON
- ⬇️ **Download** your map as `drawings.geojson`
- 📑 **Layers Control**
  - Public Hunting Lands (ODNR)
  - Ohio Counties (ODOT)
  - My Drawings
- 🌅 **Legal Light Panel** – sunrise, sunset, civil dawn/dusk, day length (based on map center)
- 🔲 **Fullscreen Toggle**

## File Overview
- `index.html` → Main web app (map + UI + scripts)
- `README.md` → This documentation

## Data Sources
- **Public Hunting Lands (ODNR)**  
  Served from:  
  `https://gis2.ohiodnr.gov/ArcGIS/rest/services/OIT_Services/DNR_Fed_Lands_Nav_Base/MapServer/2/query?where=1=1&outFields=*&f=geojson`

- **Ohio Counties (ODOT)**  
  Served from:  
  `https://gis.dot.state.oh.us/arcgis/rest/services/Basemap/ODOT_Basemap/MapServer/165/query?where=1=1&outFields=County_Name&f=geojson`

Both layers load dynamically as GeoJSON.

## Deployment
1. Push files to a public GitHub repository.
2. In repo settings, enable **GitHub Pages** → set branch = `main` and folder = `/root`.
3. Your map will be live at:  
   `https://<username>.github.io/<repo>/`

## Embedding into Wix
1. Copy the GitHub Pages link.
2. In Wix editor, add an **Embed → Embed a Site (URL)** block.
3. Paste your GitHub Pages URL.
4. Resize the block to fit the map.

## Local Testing
You can also open `index.html` directly in your browser, but note:
- Remote GeoJSON layers may not load properly from `file://` URLs.
- Use a simple local web server (e.g., `python -m http.server`) for reliable testing.

---

🚀 This repo provides a HuntWise-style base map for Ohio hunters, with live data layers and drawing tools. Future enhancements (icons, measurement tools, marker lists, multi-area saves) can be layered on top once the stable version is embedded successfully.
