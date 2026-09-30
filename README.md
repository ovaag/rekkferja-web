# rekkferja-web

Public pages for the **Rekk ferja** iOS app. The app source is in a separate
private repository.

This repository exists because App Store Connect needs public URLs:

- `privacy.html` — the privacy policy URL, required for TestFlight external
  review and for App Store submission.
- `index.html` — a landing page. It can also serve as the Support URL, which
  App Store submission requires.
- `app-config.json` — read by the app at launch and on each return to the
  foreground. A build numbered below `minimumBuild` shows «Oppdater appen»
  instead of the tabs, with a button to `updateURL` (`itms-beta://` opens
  TestFlight while the app is not in the App Store). Build numbers are the
  CI run numbers. Raise it to retire old builds; lowering it lifts the block
  on the next launch. GitHub Pages caches for about ten minutes.

GitHub Pages serves the files from the `main` branch, root directory.
