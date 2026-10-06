# Changelog

Font Scaling Lab is versioned to match the version published to the Figma Community, which Figma assigns.
A design system update is committed without a release (`build: ds-core vX.Y.Z`) and ships with the next version published.

(Some earlier entries use decimals like `v5.1` for repo-only releases. That scheme was retired on 22 July 2026.)

### v7 · 1 August 2026

- Improved clipping detection to identify the underlying cause.
- Layers outside the selected frame are now flagged in the list.
- Added more precise fix suggestions and support for additional use cases.

### v6 · 22 July 2026
Published to Figma Community.
- Added tooltips for objects outside the visible area.
- Fixed minor UI issues and improved overall polish.

Landed since publishing, and going out with the next Community release:
- The plugin now finds the real cause of clipping instead of blaming the nearest
  container. It follows the whole layer chain to the tightest constraint, whether
  that's a fixed size, a max-width several levels up, or the selected frame itself,
  and its suggestion matches the axis that actually overflowed. Font-size sources
  (variable, style, or override) read correctly again, and "View on Canvas" now
  jumps to the layer you need to change rather than the one that looks broken.
- Layers outside the selected frame are now flagged in the list.
- Failures are reported as a toast in the corner instead of a red bar wedged into
  the panel. The old bar stayed on screen after the problem had passed.
- Dark mode colours updated against the design system. The greys shifted slightly
  across the whole ramp, so panels, borders and text all move together.
- The scale stepper, the issue highlight and the suggested fixes are the design system's own
  stepper, input, highlight selector, highlight and list rows, so they match the design exactly.
- The issues list and the details panel are the design system's panel, and the close and
  generate buttons use its close and refresh icons.
- The scale field's border was too dim in dark mode and slightly too thin, and its
  focus ring used a text colour instead of the design system's focus colour.
- Spacing throughout the issue list and details panel snapped onto the design
  system's scale, replacing loose numbers that matched nothing in the system.
- Loading spinners are a pixel larger, matching the size of the design system's
  spinner rather than the shape drawn inside it.
- The info button on an issue row sits flush against its title instead of a step
  away, matching the design system.
- The "Suggested Fixes" heading uses the design system's secondary text colour and
  size — it had been the brighter primary colour and a step too large.
- The info icon was redrawn in the design system (a solid mark rather than an
  outline); the plugin now matches.

### v5.2 · 22 July 2026
Repo only, not republished to the Community.
- Section dividers are 2px taller, matching a spacing change in the design system.

### v5.1 · 22 July 2026
Repo only, not republished to the Community.
- Picks up the shared design-system fixes (node and empty-state colours).

### v5 · 4 June 2026
Published to Figma Community.
