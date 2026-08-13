# Keyboard Studio Website

Official marketing, privacy, legal, and support website for **Keyboard Studio**,
a private customizable keyboard for iPhone and iPad.

Production domain: [https://keyboardstudio.de5.net](https://keyboardstudio.de5.net)

GitHub: [yaoyiping2008-dev/keyboardstudio-site](https://github.com/yaoyiping2008-dev/keyboardstudio-site)

This repository is a standalone public website. It is not the iOS application
repository.

## Stack

- Astro static site (`output: 'static'`)
- TypeScript where appropriate
- Plain / component-scoped CSS
- No React, SSR, database, auth, cookies, analytics, advertising, or tracking
- No external font CDN and no third-party UI framework
- No runtime network requests except normal page and asset loading

## Local setup

```bash
npm install
npm run dev
```

Open the local URL printed by Astro (typically `http://localhost:4321/`).

## Scripts

| Command | Purpose |
| --- | --- |
| `npm run dev` | Local development server |
| `npm run build` | Production build to `dist/` |
| `npm run preview` | Preview the production build |
| `npm run check` | Astro + TypeScript check |

## Cloudflare Pages

| Setting | Value |
| --- | --- |
| Build command | `npm run build` |
| Build output directory | `dist` |
| Root directory | repository root |
| Node.js | 22.x recommended (`engines.node` ≥ 22.12.0) |
| Production domain | `keyboardstudio.de5.net` |

## Support email

Public support address (resolved):

```text
support@keyboardstudio.de5.net
```

Defined in `src/consts.ts` and linked via `mailto:` on Privacy, Support, Terms,
and the site footer.

Cloudflare Email Routing was manually tested successfully for inbound delivery to
this public address. Retest the address periodically to confirm forwarding still
works. Do not publish private forwarding destinations on this website.

## Release checklist

See [SITE_RELEASE_CHECKLIST.md](./SITE_RELEASE_CHECKLIST.md).

## Routes

- `/` — Homepage
- `/privacy/` — Privacy Policy
- `/support/` — Support
- `/terms/` — Terms of Use
- Custom styled `404` page

## Product wording notes

- Paid App Store download: pay once, no subscription, no In-App Purchases, no advertising
- Do not claim App Store availability before launch; use “Coming to the App Store”
- Full Access is optional; Keyboard Studio uses it for supported local sharing and feedback
- Typed text, swipe paths, and Emoji searches are processed locally and are not uploaded by Keyboard Studio
- No account, cloud typing service, analytics, behavioral tracking, or advertising
