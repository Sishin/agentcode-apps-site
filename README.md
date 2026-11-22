# AgentCode Apps website

Static site for https://agentcode-apps.web.app (Firebase Hosting). No build step.

- `public/index.html`: home page with every app
- `public/learn-kannada/`: Learn Kannada product page (screenshots and icon in `img/`)
- `public/assets/`: shared stylesheet (`site.css`) and app icons
- `public/privacy.html`: privacy policy served at `/privacy` (kept from the previous site)
- `public/app-ads.txt`: AdMob app-ads.txt (kept from the previous site)

Preview locally:

    cd public && python3 -m http.server 5178

Hosting: GitHub Pages. Every push to `main` runs `.github/workflows/pages.yml`, which publishes the `public/` folder.

Custom domain: set it in the repo under Settings > Pages > Custom domain, then add the DNS records GitHub shows there. (A CNAME file is not used with Actions-based deploys.)

`firebase.json` and `.firebaserc` are kept in case you want to deploy to Firebase Hosting instead.
