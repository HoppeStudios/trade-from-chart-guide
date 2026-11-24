# Contributing

Thanks for improving Hoppe Studios’ independent Trade From Chart installation guide. Read the [code of conduct](CODE_OF_CONDUCT.md); send sensitive reports through [the security policy](SECURITY.md), not public issues.

## Keep the scope clear

Useful contributions include factual corrections, clearer installation steps, accessibility fixes, responsive layout improvements and reproducible guide-site bug reports. Product licensing, extension defects and trading support belong with the publisher.

For a normal issue, describe the guide URL or section, expected and actual behavior, browser/version and relevant steps. Redact personal information from screenshots. Never include credentials, account identifiers or private trading data.

## Make a focused pull request

1. Fork the repository and create a branch for your change.
2. Edit the relevant source. `index.html` contains the guide’s markup, styles and JavaScript; there are no package dependencies or build step.
3. Open `index.html` locally, or run `python -m http.server 8000 --bind 127.0.0.1` from the repository directory if Python is available. Visit http://127.0.0.1:8000 and stop the temporary preview with Ctrl+C.
4. Run the checks below. Explain what changed, why, and what you actually checked in the pull request. Include website screenshots for visual changes when useful.

## Checks before submitting

- Run `git diff --check` for whitespace errors.
- Read the changed prose and verify relative links, image paths, external destinations and any section anchors you changed.
- Check desktop and narrow/mobile layouts for overflow and readable text. Test keyboard navigation, visible focus, useful image alt text and accessible link/button names.
- For guide JavaScript changes, check the browser console and the affected interactions, including the checksum-copy control when relevant.
- Keep the site static: no unnecessary dependencies, tracking, secrets or third-party binaries. There is no checked-in automated test suite; describe manual checks honestly.
- Preserve `google14435e65ea93760b.html` and its inclusion in the Pages deployment allowlist. The public payload is `index.html`, `robots.txt`, `sitemap.xml`, `.nojekyll` and that verification file; README assets are repository-only.

These checks validate the guide, not the extension’s runtime or trading behavior. Do not claim a browser or extension test you did not perform.

## Downloads, releases and rights

When changing a download reference, inspect the upstream manifest and verify the archive SHA-256. Cite the source and distinguish confirmed facts from assumptions. Do not invent publisher changelogs or label a version “latest” without evidence. A matching checksum is not proof of safety or publisher authenticity.

Guide release tags such as `guide-v1.0.0` describe this website, not the third-party extension. Link to the publisher’s download; do not add extension ZIPs or source to this repository. Do not add copyrighted artwork, trading records or screenshots you lack permission to share. Website screenshots must be identified as guide previews, not extension runtime evidence.

Hoppe-authored guide/site material is covered by the [MIT license](LICENSE). Submit only material you have the right to contribute under that license; identify any third-party material and its applicable terms in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md). No license to the extension or third-party trademarks is granted.
