# Changelog — GeneXus Work With for KB Editor

This project adheres to [Semantic Versioning](https://semver.org/).

## [0.1.4] - 2026-07-01

### Fixed
- **Activation-ordering resilience.** No longer warns that KB Editor lacks the pattern
  extensibility API when the extension merely activated before KB Editor finished exposing it;
  it now retries for a short window and registers its providers once KB Editor is ready.

## [0.1.3] - 2026-07-01

### Added
- Bundle the `Event` icon (used by the `Actions` / `Action` / `Modes` nodes). It lives in a
  different GeneXus assembly than the rest of the Work With icons, so it was missing from the
  initial icon set and those nodes fell back to a generic glyph; they now render the real icon.

## [0.1.2] - 2026-07-01

### Added
- **Node icons.** The pattern tree now renders the Work With pattern's real icons.
  They are bundled with the extension and delivered to KB Editor via the new
  `getNodeIcon` hook (as `data:` URIs), so they render without the GeneXus SDK or
  .NET assemblies on the client. Requires a KB Editor build that calls `getNodeIcon`.

## [0.1.1] - 2026-07-01

### Changed
- More robust activation and a clear warning when KB Editor is outdated and does not
  expose the pattern extensibility API.

## [0.1.0] - 2026-06-30

### Added
- Initial release. Providers for the GeneXus `WorkWith` pattern in KB Editor:
  custom type `GridCustomRender`, dynamic caption for the `Modes` node, and the
  "Add Filter Variable" command on `FilterAttributes`.
