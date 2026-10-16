# Cine Lanka — GitHub Pages starter

Includes a responsive catalogue, search, genre filters, Sinhala/English toggle, YouTube player dialog, and starter Privacy Policy and Contact pages.

## Video IDs and rights
Sample `videoId` values are intentionally `null`. Before adding one, verify the video is from an official source and embedding is permitted. Only use `videoType: "licensed-full"` if you have explicit rights to stream the complete movie on your website and in your target territory. A publicly visible YouTube URL does not itself prove redistribution or monetization rights.

To add a verified video, edit an item in `index.html`:
```js
{title:"Example Movie",year:2025,genre:"Drama",rating:"—",image:"https://example.com/poster.jpg",videoId:"ABCDEFGHIJK",videoType:"official-trailer"}
```
Replace the sample ID with the actual 11-character ID from a verified official YouTube video.

## Publish to GitHub Pages
1. Unzip this project.
2. In your GitHub repository, upload/replace `index.html`, `privacy.html`, `contact.html`, and `README.md` in the same root folder as the currently published `index.html`.
3. Commit the files to the branch/folder configured under **Settings → Pages**.
4. Wait for deployment to complete, then refresh the published site.
5. Replace starter Privacy Policy and Contact text with accurate details before launch.

This is still a static front end: no database, user accounts, payments, uploads, or private video hosting. Never commit secret API keys. Choose hosting/video services whose terms allow your intended streaming use.
