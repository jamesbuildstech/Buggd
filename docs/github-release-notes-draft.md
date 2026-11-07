# Buggd v1.1.0 — GitHub release notes (draft)

> **Draft for an official GitHub Release.** The `getbugged@1.1.0` npm package is published and its public `npx getbugged` installation has been tested. A GitHub Release has not yet been created. The product and executable are still Buggd / `buggd`.

## Find what’s broken

Buggd is a free, MIT-licensed, local-first website scanner for people who build and maintain websites. Scan sites you own or have permission to test, inspect real Chromium evidence, and work through potential problems in a visual dashboard. No accounts, telemetry, cloud storage or mandatory AI.

## Highlights

- **Discover and inspect pages:** bounded same-origin crawling, broken links and missing resources, browser errors, placeholders and common document checks.
- **Understand findings:** Simple and Technical modes, plain-English explanations, individual affected elements and evidence-backed screenshots.
- **Test across screen sizes:** desktop, tablet and mobile checks with measured highlights and explicit capture limitations.
- **Check safer interactions:** recognised nondestructive controls and native form validity, without submitting forms.
- **Fix and verify:** save review progress, rescan and compare findings with conservative coverage-aware resolution rules.
- **Keep results local:** export HTML, PDF and JSON reports; manage saved scan history and inspect the discovered page map.
- **Choose light or dark:** Buggd’s olive/lime visual identity and self-hosted typefaces.

## Install from npm

Requires Node.js 22.12+ and npm.

```sh
npx getbugged
```

If the Playwright browser is missing, use the guided setup or run `npx getbugged --install-browser`.

## Build from source

Requires Node.js 22.12+ and Git.

```sh
git clone https://github.com/skillman85/Buggd.git
cd Buggd
npm ci
npm run browser:install
npm run build
npm start
```

Buggd starts a local dashboard and prints its address. Only scan websites you are authorised to test.

**Live npm package:** [`getbugged@1.1.0`](https://www.npmjs.com/package/getbugged) has been published and the public installation command tested.

## Tested

The v1.1.0 source passed real GitHub Actions checks on Windows, Ubuntu and macOS, each with Node.js 22 and 24. The matrix includes 71 unit/integration tests, 25 browser tests, typecheck, lint, build and compiled-package/CLI smoke checks. See [CI run](https://github.com/skillman85/Buggd/actions/runs/40932911586) and [release-readiness report](final-release-readiness.md).

## Scope and limitations

Buggd is not a comprehensive accessibility, SEO or security audit. It deliberately excludes destructive actions, live form submissions, authenticated journeys and some cross-origin content. Browser screenshots may contain private information: inspect reports before sharing. See [security and coverage limits](security.md).

## GitHub Release checklist

- [x] Publish the unscoped `getbugged@1.1.0` npm package.
- [x] Verify the public `npx getbugged` install works.
- [x] Update the README to link to the live npm package and installation command.
- [x] Add reviewed Buggd UI screenshots to the README.
- [ ] Create an official GitHub Release using the verified release notes.

Buggd is [MIT licensed](../LICENSE). Contributions and bug reports are welcome via [GitHub Issues](https://github.com/skillman85/Buggd/issues).
