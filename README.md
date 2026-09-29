# Kerala-Kams

A multilingual job portal frontend for workers in Kerala.

## Deploy to Vercel

1. Extract this ZIP.
2. Push the contents of the kerala-kams folder to a new GitHub repository.
3. In Vercel, import that repository.
4. Use Framework Preset: Other; Root Directory: repository root; Output Directory: dist; Build Command: empty.
5. Deploy. The included vercel.json configures the static deployment.

No npm install or build step is needed.

## Files

- dist/index.html: markup
- dist/style.css: responsive styles
- dist/app.js: translations, sample jobs, filters and UI behavior
- dist/icon.svg: favicon
- vercel.json: deployment configuration

## Current scope

This is a frontend prototype with fictional sample jobs. Employer registration, phone OTP, Google authentication and real employer contact details are NOT connected. Registration screens are clearly labelled previews. No backend or authentication secrets are included.

Language preference, dismissed first-visit guidance and saved sample jobs are stored in this browser only. Location permission is optional. Geolocation sorts sample jobs using approximate district positions and is not saved. The site is not yet an installable PWA.

A fresh Vercel origin has separate browser storage from the current hosted preview. Its first-visit popup will therefore appear again.

## Local preview

With Python installed, run from the project directory:

    python -m http.server 8000 --directory dist

Open http://localhost:8000 in your browser.

## Changes

Edit the files in dist, commit, and push to GitHub. The linked Vercel project deploys subsequent pushes according to its configured production branch.
