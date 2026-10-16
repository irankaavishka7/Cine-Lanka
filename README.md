# Cine-Lanka — Movie Details & Official Video Player

## Features
- Responsive dark movie catalogue with hover and entrance animations
- Search and genre filters
- Movie details modal
- Responsive YouTube privacy-enhanced embedded player
- Fallback link to YouTube when no video ID is connected
- Accessibility labels and reduced-motion support

## Connect a video you are authorized to embed
Open `index.html`, find the `const movies = [...]` list, and replace the empty `videoId` value for the relevant movie with the 11-character YouTube video ID. For example:

`videoId: "M7lc1UVf-VE"`

Only use videos you own or are authorized to embed. This sample intentionally does not assume that full movies are available or licensed. Some videos may disallow embedding or be region/age restricted.

## Publish on GitHub Pages
Upload `index.html` to the root of your repository, replacing the old file. Then open **Settings → Pages**, select the `main` branch and `/(root)` folder, and save. Wait for deployment.

## Notes
This is a static front-end. It does not include a database, user accounts, payments, or an admin dashboard.
