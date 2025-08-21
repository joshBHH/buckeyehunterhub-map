# Buckeye Hunter Hub Map (GitHub Pages)

**How to publish**

1. Create a new public repo (e.g., `buckeyehunterhub-map`).
2. Upload both `index.html` and `huntingmap.html` to the ROOT of the repo.
3. In the repo: Settings → Pages → Source: Deploy from a branch → Branch: `main` / `(root)` → Save.
4. Wait ~1 minute and visit:
   - `https://<yourusername>.github.io/<repository-name>/`  (uses `index.html`)
   - or `https://<yourusername>.github.io/<repository-name>/huntingmap.html`

**Embed in Wix**

Use an Embed HTML element with:

```
<iframe src="https://<yourusername>.github.io/<repository-name>/" style="width:100%; height:600px; border:none;"></iframe>
```

If you later rename the repo, update the URL in Wix.
