BSRDCL dashboard app wrapper (GitHub Pages)
============================================
What this is: a small page that shows your Apps Script dashboard full screen and lets people install it as an app.
It holds NO data, no Google Sheet or Drive IDs. The only thing inside is the public /exec link, set in index.html (DASHBOARD_URL).

Put it on GitHub (about 5 minutes, no coding)
1. On github.com click New repository. Name it e.g. bsrdcl-dashboard. Public. Create.
2. Click "uploading an existing file". Drag in ALL of these, keeping the icons folder:
   index.html, manifest.webmanifest, sw.js, .nojekyll, icons (folder with 4 PNG files)
   Click Commit changes.
3. Settings -> Pages -> Build and deployment -> Source: "Deploy from a branch" -> Branch: main, folder / (root) -> Save.
4. After about a minute your app link appears at the top of that page:
   https://<your-github-name>.github.io/bsrdcl-dashboard/
   Share THIS link, or the original /exec link. Both work and show the same live dashboard.

Install as an app
- Android / PC (Chrome, Edge): open the GitHub link -> Install (icon in the address bar, or menu -> Install app).
- iPhone / iPad (Safari): Share -> Add to Home Screen.
After this the BSRDCL icon opens the dashboard in its own window.

If the dashboard link ever changes (new deployment gives a new /exec URL): edit index.html on GitHub (pencil icon),
change DASHBOARD_URL, Commit. Updating the SAME deployment ("Manage deployments -> Edit -> New version") keeps the link, so nothing to change.
