# Eduframe — Tuition Workflow Made Easy

## Deployment

### Netlify
1. Drag the contents of this zip into Netlify drop zone at netlify.com/drop
   OR connect your GitHub repo and set publish directory to "."

### Firebase Rules (REQUIRED — dashboard won't load without this)
1. Go to https://console.firebase.google.com/project/tution-6c2f1/firestore/rules
2. Paste the contents of firestore.rules
3. Click Publish

### Files
- index.html         — Main application (single-page app)
- firestore.rules    — Firestore security rules (deploy via Firebase Console)
- firebase.json      — Firebase CLI config
- _redirects         — Netlify SPA routing
- netlify.toml       — Netlify build & cache config
- README.md          — This file

## Fixes applied
- Dashboard blank page fixed (auth routing, null guards)
- Login functions exposed to global scope correctly
- Branding updated to Eduframe with logo
- Firestore query timeout added (8s) with clear error message
- Auth listener triple-fire fixed
