# Lab member site scaffold

Starter files for personal pages of the Cognate Speech Lab at the Reykjavík
Institute for Language Technology.

## Layout

- `_config.yml` - site metadata and the author block used by the profile card.
- `_pages/about.md` - the personal page shown at `/about/`.
- `_pages/cv.md` - a longer CV page.
- `_publications/` - one Markdown file per publication, rendered as a collection.
- `assets/tool-spec.json` - machine-readable description of a lab software package.
- `_data/type_labels.yml` - display labels for parameter types.
- `_includes/tool-doc.html` - documentation widget for the tool spec.
- `_data/navigation.yml` - top navigation entries.

## Tool documentation

Every entry under `tools` in `assets/tool-spec.json` is rendered by
`_includes/tool-doc.html`. Parameter types are looked up in
`_data/type_labels.yml`; anything that is not present in that table is
displayed as-is. The `assets/` files are consumed by the docs widget
directly - there is no intermediate schema conversion step in the build.
