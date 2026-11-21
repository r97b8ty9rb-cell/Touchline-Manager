# Touchline Manager V22.6

This release corrects the attack-end artwork transform. The embedded pitch artwork has its goal on the LEFT, so the pitch is mirrored when the active attack direction is RIGHT. The advertising banner is redrawn in normal screen coordinates after the pitch transform so its lettering remains readable. Players, goalkeeper and ball continue to use the same shared attack-direction mapping.

The release keeps the existing game, management screens, career-save storage and match presentation. The service-worker cache has been advanced to `touchline-manager-v22-6`.

## Install on iPad / GitHub Pages
1. Unzip `V22.6.zip`.
2. In the GitHub Pages repository, upload/replace `index.html`, `sw.js`, `manifest.webmanifest`, and the `icons` folder (keep the filenames and folder structure exactly as supplied).
3. Commit the changes and wait for the Pages deployment to finish.
4. Close the old Safari game tab and reopen the site. If an older version remains, reload the site or open it with `?v=22.6` added to the address.
5. Check both attack directions: home attacks right in the first half and left in the second; away attacks the opposite way. Confirm the goal is always at the attacking end and the banner text stays readable.

## Verification note
The embedded artwork was inspected and confirmed to have its goal on the LEFT. The direction transform was corrected accordingly, and the JavaScript syntax and package contents were checked. A full live match animation in iPad Safari has not been independently verified in this build.
