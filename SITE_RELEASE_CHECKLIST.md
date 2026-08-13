# Keyboard Studio Site Release Checklist

Complete every item before treating [https://keyboardstudio.de5.net](https://keyboardstudio.de5.net) as production-ready.

## Content blockers

- [x] Public support email configured in `src/consts.ts`
- [x] Public support email set to `support@keyboardstudio.de5.net`
- [x] Confirm Privacy, Support, and Terms show a working `mailto:` link
- [x] Confirm the old email placeholder token is absent from source and `dist/`
- [x] Cloudflare Email Routing inbound forwarding manually tested successfully
- [ ] Periodically retest `support@keyboardstudio.de5.net` delivery
- [ ] Search for other placeholders (`TODO`, `PLACEHOLDER`, `example.com`) and resolve them
- [ ] Verify all legal copy on `/privacy/` and `/terms/`
- [ ] Confirm Home, Privacy, Support, Terms, Footer, and README privacy claims remain consistent
- [ ] Confirm product claims remain accurate (no App Store availability claim before launch)

## Functional checks

- [ ] Test `/`
- [ ] Test `/privacy/`
- [ ] Test `/support/`
- [ ] Test `/terms/`
- [ ] Test custom `404` page
- [ ] Validate HTTPS on the production domain
- [ ] Check layout and typing flows on mobile Safari
- [ ] Check layout on desktop browsers
- [ ] Confirm no horizontal overflow on narrow and wide viewports
- [ ] Confirm skip-to-content and keyboard focus styles work

## SEO and assets

- [ ] Verify sitemap at `https://keyboardstudio.de5.net/sitemap-index.xml`
- [ ] Verify `https://keyboardstudio.de5.net/robots.txt`
- [ ] Verify App Icon at `/app-icon.png` (unaltered official icon)
- [ ] Verify favicon and apple-touch-icon
- [ ] Spot-check titles, descriptions, and canonical URLs

## Deploy

- [ ] Deploy with Cloudflare Pages
- [ ] Build command: `npm run build`
- [ ] Output directory: `dist`
- [ ] Bind custom domain `keyboardstudio.de5.net`
- [ ] Test production access in an incognito / private window
- [ ] Record final URLs in KeyboardStudio iOS release docs

## Final confirmation

- [ ] No iOS source code, signing data, App Group files, or private user data in this repo
- [ ] No analytics, advertising, cookies, account system, database, or remote API calls added
- [ ] Private forwarding destinations are not published on this website
- [ ] Site is ready for public launch
