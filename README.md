# SigneyScore ads config

Remote switch for the in-app banner ad (fixed66). The app fetches this
file on launch from:
https://raw.githubusercontent.com/signeyscore/signeyscore-ads-config/main/ads-config.json

- `"ads": false` (default) — no banner, the app looks exactly like fixed65.
- `"ads": true` — the thin banner appears at the bottom of the board
  screen only, for every user, including users who never update the app.

`adUnitId` is the AdMob banner ad unit. The value here is Google's
official TEST banner ad unit. When Signey gets a real AdMob account,
replace it with the real ad unit ID — no app update needed, just push.

To turn ads on or off: edit `ads-config.json`, commit, push. The app
picks it up on next launch (it re-checks once per session).
