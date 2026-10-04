# Font Scaling Lab

[![build](https://github.com/rafaelmatosdasilva/rms-figma-font-scaling-lab/actions/workflows/build.yml/badge.svg)](https://github.com/rafaelmatosdasilva/rms-figma-font-scaling-lab/actions/workflows/build.yml)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

**Stress test layouts under text scaling**

[Open in Figma Community →](https://www.figma.com/community/plugin/1632816540279283797/font-scaling-lab)

Typography systems often work well under ideal conditions but break in real use.
Text resizing, assistive technologies, and changing content cause overflow, broken
layouts, and lost hierarchy. Font Scaling Lab simulates these conditions so you can
test how your typography behaves beyond fixed assumptions.

- No setup required — runs safely on existing layouts without modifying any values.
- Simulates realistic text scaling to mimic zoom and accessibility settings.
- Detects truncation, clipping, and constraint failures caused by fixed dimensions.
- Suggests targeted fixes for each detected issue.

![Font Scaling Lab](docs/preview.png)

It runs entirely inside your Figma file with no network access, no data sent anywhere, and no third party code.
It's built on the [RMS design system](https://github.com/rafaelmatosdasilva/rms-ds-figma-plugins), which lists
every plugin and product made with it.

Click **Watch → Custom → Releases** to be notified about new versions.

## Install

1. Go to [Releases](../../releases) and download the latest zip,
   e.g. `font-scaling-lab-v7.zip`. Unzip it.
2. In the Figma **desktop** app: **Plugins → Development → Import plugin from
   manifest…**
3. Pick the `manifest.json` inside the unzipped folder.

That's it. Nothing to install, nothing to build. Run it any time from
**Plugins → Development**.

Prefer the source? Clone this repository, or use the green **Code** button → **Download ZIP**,
and point step 3 at its `manifest.json`.

**Needs the desktop app.** Figma in a browser has no **Plugins → Development**
menu, so sideloading isn't possible there. Once imported, the plugin runs on
design files — not FigJam or Slides.

## Get updates

Download the new zip from [Releases](../../releases) and replace the folder, or
`git pull` if you cloned. Reopen the plugin and you're on the new version.
Re-import the manifest only if the folder moved.
[CHANGELOG.md](CHANGELOG.md) lists what changed.

The version matches the plugin's version on the Figma Community. The plugin logs it on startup,
under **Plugins → Development → Open console**.

## Building from source

Only needed if you change the code. Requires Node 24 and pnpm:

```sh
pnpm install
pnpm build
pnpm test
```

The design system (theme, shared UI and the build tools) comes from
[rms-ds-figma-plugins](https://github.com/rafaelmatosdasilva/rms-ds-figma-plugins), at the version pinned in
`package.json`. A new design system release updates, rebuilds and releases this plugin automatically.

## Contact

Feedback and ideas are welcome:

- Email — [hello@rafaelmatosdasilva.com](mailto:hello@rafaelmatosdasilva.com)
- LinkedIn — [rafaelmatosdasilva](https://www.linkedin.com/in/rafaelmatosdasilva/)

## License

MIT — see [LICENSE](LICENSE).
