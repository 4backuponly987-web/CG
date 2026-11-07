# Common Ground — iPhone / GitHub Pages Offline Build

This folder is ready to upload directly to a GitHub repository and publish with **GitHub Pages**.

## Install on iPhone
1. Upload all files in this folder to the root of your GitHub repo.
2. In GitHub: **Settings → Pages → Deploy from a branch → main / root**.
3. Open the Pages URL in **Safari** on the iPhone while online.
4. Play/open the game once so the service worker can cache it.
5. Tap **Share → Add to Home Screen → Add**.
6. Launch it from the Home Screen. After the initial cache, the game is designed to work offline.

## iPhone changes
- Standalone Home Screen PWA metadata and icons.
- Entire game cached for offline play.
- Safe-area support for notches / Dynamic Island.
- Touch targets and small-screen layout hardened for iPhone.
- Text/image highlighting and Safari long-press callouts disabled outside real text fields.
- Pinch zoom and double-tap zoom blocked during play.
- Inputs stay at 16px or larger to prevent Safari auto-zoom when the keyboard opens.
- Existing game modes, local-party logic, scores and content are preserved.

## Updating
If you upload a later build, update the cache name in `service-worker.js`, then open the Pages version once while online before testing offline again.
