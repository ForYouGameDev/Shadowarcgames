SHADOW ARC GAMES — WEBSITE STARTER

HOW TO RUN
1. Extract this folder.
2. Open index.html in a modern browser. No server or build tools are required.
3. Edit games.js to add, remove or update games.
4. Edit stories.js to add optional story pages/sections.
5. Put your images in assets/ and update the matching image paths.

ADD A GAME
Copy one object in games.js and edit:
- id: unique lowercase ID (use hyphens)
- title, genre, tagline, description
- status: 'released' or 'coming-soon'
- storeUrl: exact Google Play URL, e.g. https://play.google.com/store/apps/details?id=YOUR.PACKAGE
- cover: image path, e.g. assets/my-game.jpg
- featured: true or false
- storyId: matching story ID, or '' if there is no story

COMING SOON
Set status to 'coming-soon'. You can leave storeUrl blank; the website will show a Coming Soon label. If you later add a Play Store URL, the card automatically becomes downloadable.

ADD A STORY (OPTIONAL)
1. Add a story object in stories.js with a unique id, gameId, title, subtitle, cover and paragraphs array.
2. Set that game's storyId in games.js to the same story id.
3. A Read Story link will appear on its game card and open a dedicated story view.

ADD YOUR LOGO
1. Save your logo as assets/studio-logo.png.
2. In index.html, find the .brand-mark element and replace the SA text mark with:
   <img src="assets/studio-logo.png" alt="Shadow Arc Games logo">
3. Adjust .brand-mark img width/height in the CSS if needed.

PUBLISH
Upload the complete folder to any static website host (for example GitHub Pages, Netlify or your own hosting). Keep index.html, games.js, stories.js and assets together. This starter does not include a backend or admin login; edit the data files and re-upload to publish changes.
