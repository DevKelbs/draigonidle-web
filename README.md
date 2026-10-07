# draigonidle.com

The website for **Draigon Idle**, an idle guild game for iPhone.

Built with [Astro](https://astro.build) and deployed to [Cloudflare Pages](https://pages.cloudflare.com/). Pushing to `main` deploys it.

## Run it

Needs Node.js 22.12 or later.

```sh
npm install
npm run dev       # http://localhost:4321
npm run build     # the built site lands in dist/client
npm run preview
```

## Where things are

```
src/data/site.ts        Links, price, version, contact address. Change these here, not in the pages.
src/layouts/            BaseLayout.astro: the page shell (head, header, footer)
src/components/         Header, Footer, Contact (email if there is one, Discord if not)
src/pages/              index, patch-notes, press-kit, privacy, terms
src/styles/global.css   All the styling. The colours match the game's.
public/images/          Pixel art and trailer scenes, made from the game's own sprites
public/video/           The trailer
```

## Things to fill in

All in `src/data/site.ts`:

- `appStoreUrl`: once the game is on the App Store. The "Join the beta" buttons turn into "Get it on the App Store".
- `testFlightUrl`: a public TestFlight link, if there is one. Until then the beta button goes to Discord.
- `discord`: must be an invite that never expires. It's also the contact for privacy, legal and press questions: there's no mailbox.
- `legalUpdated`: change it whenever the privacy policy or terms change.

## Patch notes

Add a release to the top of the `releases` list in `src/pages/patch-notes.astro`.
