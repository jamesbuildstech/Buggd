# Future work

## Current status

Buggd v1.1.0 source is available on GitHub, with six GitHub Actions jobs passing on Windows, Ubuntu and macOS with Node.js 22 and 24. See the [final release-readiness report](final-release-readiness.md).

**Public npm publication is pending.** The unscoped `buggd` package name was rejected by npm’s similarity protection; the maintainer has requested manual review and prepared `getbugged` as the alternative unscoped npm name. The product is still called Buggd, and its executable stays `buggd`. Do not claim `npx getbugged` is publicly installable until npm accepts publication and a clean install succeeds.

## Near-term

- Verify npm accepts the unscoped `getbugged` package name, publish the reviewed package under that name, and test `npx getbugged` from a clean environment without changing Buggd branding.
- Add privacy-reviewed application screenshots from a fresh authorised Buggd scan.
- Collect issue reports from actual users and improve first-run guidance based on observed difficulties.

## Possible future enhancements

- Authorised iframe inspection and clearer closed-shadow-root coverage.
- Broader opt-in interaction and custom validation fixtures without weakening write/network locks.
- More identity migration strategies when sites replace or restructure elements; ambiguous cases must remain unverified.
- Additional localisation/font subsets and assistive-technology testing.
- Broader real-world HTTPS/CDN fixtures, browser resource budgets and large-site map/evidence usability.
- Designer source vectors, if available, to replace the close reconstruction of the approved brand image.

These items are ideas, not promises or claims of current functionality.
