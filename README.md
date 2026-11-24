# Boom & Defend – website

Public pages for the game **Boom & Defend** (`com.boomdefend.game`, Android, iPhone and browser):

- `index.html` – start page
- `privacy-policy.html` – privacy policy (English + German)
- `impressum.html` – Impressum
- `img/`, `fonts/` – web images and the Baloo 2 font (served from here: no outside requests)
- `store/` – store listing graphics (Google Play; `store/ios/` App Store)

The pages are generated from the game's source (`python3 scripts/site-images.py` and
`npm run legal` in the game repository, then copy `docs/` here); edit them there, not here.

Live site: https://boomanddefend.com/ (custom domain via `CNAME`; DNS at Strato: A record `185.199.108.153`, `www` CNAME `felixsecondary03.github.io`; the old github.io address redirects there)

## play/ (challenge links)

`play/` is the game's web build. Challenge links shared from the app (`/play/?c=d2026-11-24&s=12450`:
a day's daily, `cw…` a week's weekly towers, `cl3-2` a campaign level, `s` the score to beat) open it
on that challenge. Update it from the game repo: `npm run build && node scripts/site-play.mjs`.
