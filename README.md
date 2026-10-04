# Dr. Kaung — Three.js product website

Latest reference-based version, exported 4 October 2026.

## Included
- index.html: full product page, Myanmar/English content
- style.css: responsive design
- app.js: Three.js geometry, lighting, controls, ingredient selection
- assets/: all photos, label textures, reference sheets, local Three.js modules and its MIT license
- .nojekyll: allows direct static hosting on GitHub Pages

No installation, bundling, API key or backend is required. The website uses locally included Three.js 0.186.1 modules.

## Run locally
From this folder run:

    python -m http.server 8000

On Windows you may use:

    py -m http.server 8000

Open http://localhost:8000 in your browser. Do not open index.html by double-clicking: browser security can block ES modules and textures over file://.

## Upload to GitHub
1. Create a repository, for example dr-kaung-website.
2. Extract this ZIP.
3. Upload the CONTENTS of the Dr-Kaung-3D-Website folder to the repository root. Keep index.html and assets/ at the same level. Upload extracted files, not the ZIP itself.
4. Commit the files to main.

If the browser upload limit is reached, upload assets separately or use GitHub Desktop.

## Publish using GitHub Pages
In repository Settings > Pages:
- Source: Deploy from a branch
- Branch: main
- Folder: / (root)
- Save

GitHub will display the published URL once deployment completes. GitHub Pages availability depends on your account and repository visibility. This is a separate deployment from the original private preview; configure repository and Pages visibility deliberately.

Relative asset paths allow deployment under /repository-name/ without code changes.

## Customization
- Edit text in index.html. data-en and data-my hold translations.
- Edit ingredient descriptions in app.js.
- Replace images and textures in assets/ while preserving filenames, or update references.
- Bottle and carton geometry and material settings are in start3D() in app.js.
- Add confirmed seller contact, price and delivery details in the contact section.
- The advertisement video is not included because no finished video file was supplied.

## Known limitations
The 3D model and label textures are approximations based on supplied reference sheets. Obtain original print artwork and dimensions for a production-accurate model. Small reference text may be distorted. Seller contact, prices and ordering are not configured. There is no payment or order-processing backend. JavaScript syntax and assets were checked; live browser visual testing remains pending.

## Rights
Three.js is MIT licensed; see assets/THREE-LICENSE.txt. Product branding and supplied photographs/reference images remain subject to their owners' rights. No new license is granted for those assets.
