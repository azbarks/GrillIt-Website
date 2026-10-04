# GrillIt Website — Claude Context

Static marketing / support site for the GrillIt iOS app (source: `../grillIt`).
Published as GitHub repo **GrillIt-Website** with GitHub Pages →
https://azbarks.github.io/GrillIt-Website — the app's Settings → About links to the site and
`help.html`, so keep that repo name and `help.html` filename.
Same structure as the PrayIt (`../prayer_website`) and RememberIt sites — plain HTML + one
shared `style.css`, no build step, no JavaScript.

## Pages
- `index.html` — hero (phone mockup of the Cooks list), trust bar, feature grid, how-it-works, iCloud band
- `help.html` — full guide, sidebar of sections; keep in sync with the app's behavior
- `privacy.html` — App Store privacy-policy URL
- `support.html` — App Store support URL (email azbarks@gmail.com)
- `style.css` — tokens + nav/footer/buttons. Colors from the app icon: charcoal-navy
  `#101A28`, ember orange `#D9661A`; Bitter (headings) + Source Sans 3. Light + dark.
- `images/` — `icon.png` (256, nav + how-it-works), `favicon.png`, `apple-touch-icon.png`

## At release (TODO)
- `index.html` `#download`: swap the "Coming soon" badge for the real App Store button
  (commented template is right there), and change the hero tag to "Available now on the App Store".

## Keep accurate
- **Privacy page must match the app.** GrillIt's only network call is the optional
  *Use Current Weather* (location rounded to 2 decimals → Open-Meteo; location not stored).
  Permissions: location (when in use), camera (Take Photo). Photos come through the system
  picker (no library permission). If the app adds any network call or permission, update
  `privacy.html` — and the App Store privacy labels.
- Help describes: Prepping → Start → Finish, two-grill cooks (Finish on / Move Now),
  temperature log, weather, photos (phone size ~100 KB), 1–10 stars, Cook This Again
  (copies count; clears weight), grill order / default grill, backup merge-by-id.
