# Buggd v1.1.0 — First public release

**Find what’s broken.**

Buggd is a free, MIT-licensed, local-first website testing tool. Scan websites you own or have permission to test, inspect issues backed by real Chromium browser evidence, and work through practical fixes in a visual dashboard. No account, hosted service, telemetry or mandatory AI required.

## Install

Requires Node.js 22.12+ and npm.

```bash
npx getbugged
```

The **product is called Buggd**; the npm package is **[getbugged](https://www.npmjs.com/package/getbugged)** and the installed CLI executable is `buggd`.

Buggd normally opens its dashboard locally in your browser. If Chromium has not been installed yet, follow Buggd’s setup instructions or use:

```bash
npx getbugged --install-browser
```

## Highlights

- **Find website problems:** bounded same-origin crawling, broken links, missing images and resources, browser errors, placeholders and basic document checks.
- **Understand what happened:** Simple and Technical views, plain-English explanations, evidence, element highlights and screenshots.
- **Review responsive pages:** desktop, tablet and mobile checks, with explicit evidence and coverage limitations.
- **Test cautiously:** native form validity and recognised non-destructive controls without submitting forms.
- **Track fixes:** save review progress, rescan and compare findings conservatively.
- **Keep your results local:** scan history, page maps and HTML, PDF and JSON exports.
- **Choose your theme:** light, dark and system appearance, with Buggd’s olive/lime visual identity.

## Verification

The release candidate passed 71 unit/integration tests, 25 end-to-end browser tests, lint, typecheck, a production build and a clean installed-package smoke test. Earlier cross-platform CI checks covered Windows, Ubuntu and macOS on Node.js 22 and 24. A clean `npx getbugged@1.1.0` installation was also tested successfully against the public npm registry.

## Important limits

Only scan websites you own or have authorisation to test. Buggd does not claim to be a comprehensive accessibility, SEO or security audit. It deliberately limits network access, avoids destructive actions and does not validate authenticated journeys or submitted form processing. Screenshots and exported reports may contain sensitive site content: review them before sharing.

Read [security and coverage limits](https://github.com/skillman85/Buggd/blob/main/docs/security.md) and [contributing guidelines](https://github.com/skillman85/Buggd/blob/main/CONTRIBUTING.md).

**Source:** https://github.com/skillman85/Buggd  
**npm:** https://www.npmjs.com/package/getbugged
