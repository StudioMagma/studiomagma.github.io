# Magma Studios

A lightweight static landing page for Magma Studios, presenting Puzzle World, Project Oasis, and its upcoming SinCity update.

## Goal
Introduce the studio and its games, link to the official Steam listing, and provide a directly accessible Puzzle World privacy policy for Google Play.

## File tree
```text
studiomagma.github.io/
├── index.html              Studio landing page, games, SinCity announcement, contact
├── privacy-policy.html     Puzzle World privacy policy and privacy contact
├── styles.css              Shared responsive styles, focus states, reduced-motion support
├── assets/
│   ├── mark.svg            Studio mark and browser favicon
│   ├── puzzle-world.png    Existing Android screenshot (old Block Party branding)
│   └── project-oasis.jpg   Official Project Oasis Steam artwork
├── .nojekyll               Serve files directly with GitHub Pages
└── overview.md             Documentation and manual acceptance checklist
```

## Implementation
- Plain HTML and CSS; no dependencies, JavaScript, build step, forms, analytics, cookies, or external font requests.
- Puzzle World is marked as coming to Google Play until its public store URL is available.
- Puzzle World is the public name requested by the studio; the source project remains `Puzzel`. Its existing screenshot still displays the previous Block Party name.
- Confirmed Steam page: https://store.steampowered.com/app/4970790/Project_Oasis/
- Privacy contact: fohlan@outlook.com.
- Privacy statements reflect the owner's confirmation: the game is free, without ads, purchases, accounts, analytics, or data collection. Voluntary email inquiries are disclosed separately.
- Policy date: November 17, 2026.

## Functions
None. The site uses semantic HTML, native anchors, email links, and CSS media queries; there are no application functions.

## Development plan — completed
1. Inspect game documentation and confirm studio identity, Steam link, app name, data practices, and contact email.
2. Implement the responsive landing page and separate privacy policy with locally hosted assets.
3. Review source and document deployment and manual acceptance steps.

## Validation and deployment
Source and supplied imagery were reviewed. No builds, automated tests, or browser tests were run, per workspace instructions. The local Git repository uses branch `main`. Its `origin` now points to `https://github.com/studiomagma/studiomagma.github.io.git`, replacing the personal-account remote under `iluminismo`. The organization remote was reachable and had no advertised main branch before the initial push. GitHub Pages activation and live publication are not yet verified.

Publish these root files through GitHub Pages. Once `https://studiomagma.github.io` is configured and publicly serving them, the intended privacy URL is `https://studiomagma.github.io/privacy-policy.html`. That URL is not yet verified live. Google Play requires a public policy URL and a policy link or text within the app; publishing this site does not add the in-app link or complete the Play Console Data safety form.

Requirements checked against Google's policy: https://support.google.com/googleplay/android-developer/answer/10144311

## Manual acceptance checklist
- [ ] Review the landing page on phone and desktop, including both game images.
- [ ] Check Steam, Steam news, email, page anchors, and privacy links.
- [ ] Check keyboard focus and the Skip to content link.
- [ ] Confirm Puzzle World is also the name used in the Android app and Play listing; replace the old screenshot when available.
- [ ] Confirm the policy matches the final shipped game and any SDKs it includes.
- [ ] After deployment, open the privacy URL without signing in and add it to Play Console and the Android app.

## GitHub organization setup — November 17, 2026
- Organization: `studiomagma`; repository: `studiomagma.github.io`.
- Origin fetch and push URL: `https://github.com/studiomagma/studiomagma.github.io.git`.
- Publish from repository **Settings → Pages → Deploy from a branch → main → / (root)**, then Save.
- Intended site: `https://studiomagma.github.io/`.
- Initial push was attempted but failed: HTTPS Git authentication could not obtain a username through `/usr/bin/ksshaskpass`. Authenticate GitHub in the local Git client, then run `git push -u origin main`. The organization remote is configured; uploading the commits and activating Pages remain pending.
- No site source changes, builds, or tests were needed for this Git configuration task.

Manual setup checklist:
- [ ] Confirm the website files appear in the organization repository on `main`.
- [ ] Enable Pages with `main` and `/ (root)` as the source.
- [ ] Once GitHub reports deployment complete, open the homepage and `/privacy-policy.html` without signing in.
