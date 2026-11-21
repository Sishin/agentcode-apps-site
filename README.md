# AgentCode Apps website

Static site for https://agentcode-apps.web.app (Firebase Hosting). No build step.

- `public/index.html`: home page with every app
- `public/learn-kannada/`: Learn Kannada product page (screenshots and icon in `img/`)
- `public/assets/`: shared stylesheet (`site.css`) and app icons
- `public/privacy.html`: privacy policy served at `/privacy` (kept from the previous site)
- `public/app-ads.txt`: AdMob app-ads.txt (kept from the previous site)

Preview locally:

    cd public && python3 -m http.server 5178

Deploy (publishes the live site):

    firebase deploy --only hosting

`.firebaserc` assumes the Firebase project ID is `agentcode-apps`. Check it with `firebase projects:list` before the first deploy.
