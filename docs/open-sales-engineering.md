# Open Sales Engineering website

The organization landing page lives in [`index.html`](../index.html), with
[`styles.css`](../styles.css) and [`assets/`](../assets/) alongside it.
Its artwork, screenshot, fonts, and license notices are local. There is no
JavaScript, package install, build step, analytics, or third-party request when
loading the page.

## Preview

Open `index.html` directly in a browser, or serve this repository with Python's
standard-library server from the repository root:

```sh
python3 -m http.server 8080 --bind 127.0.0.1
```

Visit <http://127.0.0.1:8080>. Stop the server with Ctrl+C.
Python is only needed for this optional server, not for direct-file previews.

## Publish

Upload `index.html`, `styles.css`, and the entire `assets/` directory to any
static host. Keep them together; `README.md` and `docs/` do not need to be
published. All asset paths are relative, so hosting at a domain root or a
subpath works without configuration. No hosting or GitHub repository
visibility is changed by this site.

Open Field Engineer's repository is currently private. The page explicitly
notes that its project and documentation links require GitHub access. Update
that notice if the repository becomes public.

## Content and assets

The page introduces the Open Sales Engineering organization and spotlights
Open Field Engineer. Project descriptions come from the
[project README](https://github.com/open-sales-engineering/open-field-engineer/blob/0fc596f375a2ae94ec806206b132f4513bbecbd8/README.md).
The project sunflower, screenshot, and MIT notice are preserved from that
repository's revision `0fc596f375a2ae94ec806206b132f4513bbecbd8`.
The site bundles:

- [`assets/open-sales-engineering.svg`](../assets/open-sales-engineering.svg)
  is the organization's font-independent monogram, used for the wordmark and
  favicon. It does not depend on a branding repository or an installed font.
- [`assets/sunflower.svg`](../assets/sunflower.svg) is the project's original
  [`apps/web/public/sunflower.svg`](https://github.com/open-sales-engineering/open-field-engineer/blob/0fc596f375a2ae94ec806206b132f4513bbecbd8/apps/web/public/sunflower.svg).
- [`assets/workbench.png`](../assets/workbench.png) is the original
  [`003-overview.png`](https://github.com/open-sales-engineering/open-field-engineer/blob/0fc596f375a2ae94ec806206b132f4513bbecbd8/docs/ui-evidence/screenshots/003-overview.png)
  from the project's UI evidence. It shows a synthetic sample workspace, not
  real customer data. The image links to its full-size local copy.
- The MIT notice is retained in
  [`assets/LICENSE-open-field-engineer.txt`](../assets/LICENSE-open-field-engineer.txt).
- Bricolage Grotesque Bold and Instrument Sans Regular are bundled unmodified
  in [`assets/fonts/`](../assets/fonts/). Their SIL Open Font License notices
  are retained in [`assets/fonts/licenses/`](../assets/fonts/licenses/).
  Keep these notices with redistributed fonts.

Edit copy in `index.html` and the palette, typography, and responsive layout in
`styles.css`. Navigation, project links, and the full-size screenshot work
without JavaScript, including when opened as a local file.
The footer credits Synctune and links to <https://www.synctune.it>.

## Checks

Before publishing, open the site directly and serve it at both a static root
and a subpath. Check widths of 320, 390, 768, and 1440 pixels for overflow,
readable copy, and visible navigation.

With JavaScript disabled, verify the skip link and section anchors using the
keyboard, and open the full-size workbench image. Check that all local assets
and links resolve, both bundled fonts load, and the browser reports no console
errors, failed requests, or external page-load requests. Keep the artwork and
font license notices with the published files. No package install or build is
required for these checks.
