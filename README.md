# mass-theme-synthwave

A [MASS](https://github.com/chinese-room-solutions/mass) /
[Grimoire](https://github.com/chinese-room-solutions/grimoire) UI theme after
the Synthwave '84 look — deep-purple surfaces, hot-pink accents, neon glows.

The whole theme is the single self-describing [`synthwave.css`](synthwave.css):
CSS custom-property declarations plus `label:` and `base:` directives, wrapped
by the apps into an `html.sl-theme-synthwave` rule. The file name (minus
`.css`) is the theme's stable id. It is indexed in
[mass-registry](https://github.com/chinese-room-solutions/mass-registry) as the
`theme-synthwave` package.

## Install

- MASS: theme picker (palette icon) → Browse themes… → Install.
- Grimoire: Extensions dialog (puzzle icon) → Themes → Install, or
  `grimoire theme install theme-synthwave`.

Both apps load themes from the shared `<user-config-dir>/mass/themes/`
directory, so installing in one makes it available to the other. Manual
install is copying `synthwave.css` into that directory.

## Publishing

1. Tag a release (`git tag vX.Y.Z && git push --tags`). The release workflow
   attaches `synthwave.css` to the GitHub Release.
2. Update the `theme-synthwave` entry in mass-registry with the release URL
   and the file's sha256 (`sha256sum synthwave.css`).

## License

Apache-2.0 — see [LICENSE](LICENSE).
