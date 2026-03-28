# draigonidle.com

Landing page for **Draigon Idle** — a dragon-themed idle game by [Stonemill Studios](https://stonemillstudios.com).

Built with [Astro](https://astro.build) and deployed to [Cloudflare Pages](https://pages.cloudflare.com/).

## Local Development

**Requirements:** Node.js >= 22.12.0

```sh
# Install dependencies
npm install

# Start dev server (http://localhost:4321)
npm run dev

# Production build
npm run build

# Preview the production build locally
npm run preview
```

## Project Structure

```
/
├── public/             # Static assets (favicon, images)
├── src/
│   ├── components/     # Reusable Astro components
│   │   ├── Header.astro
│   │   └── Footer.astro
│   ├── layouts/
│   │   └── BaseLayout.astro   # Shared HTML shell (head, header, footer)
│   ├── pages/
│   │   ├── index.astro        # Home — hero + feature highlights
│   │   ├── press-kit.astro    # Press Kit
│   │   └── patch-notes.astro  # Patch Notes
│   └── styles/
│       └── global.css         # Design tokens + global styles
├── astro.config.mjs    # Astro config (Cloudflare Pages adapter)
├── package.json
└── tsconfig.json
```

## Deployment

Auto-deploys to Cloudflare Pages on push to `main`. No manual steps required.

The Cloudflare Pages project is configured at:
- **Production branch:** `main`
- **Build command:** `npm run build`
- **Output directory:** `dist`

## Pages

| Route          | Description                        |
| -------------- | ---------------------------------- |
| `/`            | Home — hero, features, app badges  |
| `/press-kit`   | Press kit — facts, assets, screens |
| `/patch-notes` | Version history and changelogs     |

## Contributing

See the [Paperclip board](https://stonemillstudios.com) for open tasks. All changes require CTO review and board approval before pushing.
