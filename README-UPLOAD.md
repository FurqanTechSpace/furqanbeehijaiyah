# FurqanBee — Summer Edition, complete Vercel upload

## Upload to GitHub
1. Extract this ZIP first. Do not upload the ZIP itself.
2. Open the GitHub repository linked to your existing Vercel project.
3. Choose Add file > Upload files.
4. Drag ALL extracted files AND folders into the upload area. Keep their
   folder structure. At repository root you must see index.html,
   vercel.json, assets/, fonts/, icons/, media/ and vendor/ side by side.
5. Commit the files to the branch used for production in Vercel.
   Replace old files with matching paths; uploading only index.html
   or only the top-level files leaves the images/camera dependencies missing.

This package has fewer than 100 files, each below 25 MiB, suitable for
GitHub browser upload. Wait until every upload finishes before committing.
https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository

## Vercel settings
Use your existing project to keep furqanbee.vercel.app.
Root Directory: repository root (leave blank / default).
Framework Preset: Other.
Build Command: override, empty (no build).
Output Directory: . (repository root).
Install Command: empty (no installation).
The included vercel.json configures these static-site settings.
No npm, API keys, environment variables or backend are needed.
If you put everything inside a subfolder instead, Root Directory MUST
point to that subfolder containing index.html and vercel.json.
https://vercel.com/docs/builds/configure-a-build

After the GitHub commit, wait for the Vercel production deployment to
show Ready. If the repository is not connected yet, import it into
Vercel and use the same settings above.

## Check the published result
Open these paths on your production domain:
/assets/summer/flavour-2.svg (pink strawberry bowl)
/assets/wooden-jar.svg (wooden honey jar)
/media/kiko-portrait.png (transparent Kiko)
/honey-summer.css (Summer stylesheet)
/release.json (release identifier)
These should return real files, not a 404 page or the main HTML page.
Test a game and camera permission in Chrome/Edge on HTTPS.

If an earlier version is cached, click Muat versi baharu when offered.
Close and reopen old tabs. An Incognito window helps compare a fresh
load without the previously installed service worker. This release has
its own service-worker cache version and revalidation headers.

## Included
All six Summer flavour illustrations and seven topping illustrations;
wooden honey jar and dipper; Kiko/Yuyu portraits, animations and posters;
garden artwork; all game code and styles; Baloo font and license;
MediaPipe JavaScript, WASM files and hand-tracking model; manifest/icons.
No external CDN download is required for these assets.

## Player data
Rewards currently last only for the open session and reset on refresh.
Hosting does not add accounts or permanent player storage. Browser
storage or accounts/database can be added separately.

## Verification
Archive integrity, exact-case local HTML/CSS asset references, cache
entries, dynamic Summer/character assets and vendor files checked.
Actual Vercel deployment and physical webcam are not verified by this
archive check. The live domain was inaccessible from our checking tools.
