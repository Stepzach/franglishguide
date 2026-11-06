# Guide Franglish de Zach

A personal food guide to Paris and London, in English and French. Built with HTML, CSS and JavaScript, with a map, photos, likes and comments.

## Run locally

```sh
npm start
```

Open http://localhost:4173. Python 3 is required for the preview server. There is no build step or package installation.

Check the JavaScript with `npm run check` (requires Node.js).

## Publish with GitHub Pages

In this repository’s **Settings → Pages**, choose **Deploy from a branch**, then **main** and **/ (root)**. The site is ready to serve directly from this folder.

## Edit the guide

- `places.js`: places, category types, photos, addresses and English notes.
- `i18n.js`: French translations and interface labels.
- `style.css`: layout and appearance.
- `app.js`: list, language switches, place pages and comments.
- `maps.js`: interactive map controls and pins.

## Firebase

The site uses Firebase project `londonrestaurants-b7223` for anonymous sign-in, shared likes and comments. Visitors enter a display name when commenting. The public web configuration is in `firebase-config.js`; database access is controlled by `firestore.rules`.

The existing Firebase project must have Anonymous Authentication enabled and these Firestore rules published. Changing this repository does not automatically deploy the rules.

## Credits

Photos supplied by Zach, with additional images from Season and Los Mochis. Original photo sources are recorded in `places.js`.

The map uses OpenFreeMap, OpenMapTiles and OpenStreetMap data with MapLibre GL JS. The map style is adapted from Positron. Library, map-style and Newsreader font licenses are included in `assets/`. Keep the map attribution and these licenses when reusing the site.
