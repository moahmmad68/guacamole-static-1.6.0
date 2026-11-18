# Apache Guacamole 1.6.0 — static assets mirror

This repository hosts a **mirror of the static web assets** (JavaScript, CSS, fonts, and images) extracted from the official **Apache Guacamole 1.6.0** client WAR.

It is **not** a new official Apache Guacamole release, **not** a fork of the Guacamole project, and **not** affiliated with or endorsed by the Apache Software Foundation. The files here are redistributed under the terms of the [Apache License 2.0](./LICENSE) that accompanies Guacamole 1.6.0.

## Source

- Upstream project: [Apache Guacamole](https://guacamole.apache.org/)
- Client sources: [apache/guacamole-client](https://github.com/apache/guacamole-client) (tag `1.6.0`)
- Assets were taken from the real Guacamole **1.6.0** WAR build and published unchanged for CDN-style serving (for example via jsDelivr).

## Repository layout

Static files keep the same relative paths they have inside the WAR/static tree, for example:

- `guacamole.02ba1c394df380a3f7d7.js` — main Guacamole client bundle
- `1.guacamole.*.js` / `1.guacamole.*.css`
- `guacamole-common-js/all.min.js`
- `angular.min.js`, `jquery.min.js`, `lodash.min.js`, …
- `fonts/`, `images/`, …

Exactly **79** static files are published, plus this `README.md` and the upstream `LICENSE`.

## Using with jsDelivr

jsDelivr can serve files from this GitHub repository by path and tag:

```text
https://cdn.jsdelivr.net/gh/moahmmad68/guacamole-static-1.6.0@1.6.0/<path-to-file>
```

Examples:

```text
https://cdn.jsdelivr.net/gh/moahmmad68/guacamole-static-1.6.0@1.6.0/guacamole.02ba1c394df380a3f7d7.js
https://cdn.jsdelivr.net/gh/moahmmad68/guacamole-static-1.6.0@1.6.0/1.guacamole.c2fc19251fc606ad2140.css
https://cdn.jsdelivr.net/gh/moahmmad68/guacamole-static-1.6.0@1.6.0/guacamole-common-js/all.min.js
```

Prefer the `@1.6.0` tag (or another immutable ref) so the URL content does not change unexpectedly.

## Attribution

Apache Guacamole, Guacamole, Apache, the Apache feather logo, and the Apache Guacamole project logo are trademarks of the Apache Software Foundation. This mirror redistributes static assets from Guacamole 1.6.0 under the Apache License 2.0; please see [LICENSE](./LICENSE) for full terms, including notices for bundled subcomponents (for example Carlito fonts).

For the authoritative project and downloads, use [guacamole.apache.org](https://guacamole.apache.org/).
