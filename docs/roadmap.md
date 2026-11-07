# Future work

## Current status

Buggd v1.1.0 source is available on GitHub, with six GitHub Actions jobs passing on Windows, Ubuntu and macOS with Node.js 22 and 24. See the [final release-readiness report](final-release-readiness.md).

**Public npm publication completed.** Buggd v1.1.0 is published as the unscoped [`getbugged`](https://www.npmjs.com/package/getbugged) package and has been launched successfully through `npx getbugged` from the registry. The product remains Buggd and its executable remains `buggd`.

## Near-term

- Gather first-run reports from public npm installs, including browser installation on macOS, Windows and Linux.
- Keep npm release instructions and GitHub documentation aligned as new versions are published.
- Collect issue reports from actual users and improve first-run guidance based on observed difficulties.

## Possible future enhancements

- Authorised iframe inspection and clearer closed-shadow-root coverage.
- Broader opt-in interaction and custom validation fixtures without weakening write/network locks.
- More identity migration strategies when sites replace or restructure elements; ambiguous cases must remain unverified.
- Additional localisation/font subsets and assistive-technology testing.
- Broader real-world HTTPS/CDN fixtures, browser resource budgets and large-site map/evidence usability.
- Designer source vectors, if available, to replace the close reconstruction of the approved brand image.

These items are ideas, not promises or claims of current functionality.
