# KB Editor — Pattern Extensions

A catalog of **pattern extensions for KB Editor** (the GeneXus visual editor inside VS Code /
VSCodium, `kbbridge.genexus-visual-editor`) from different providers. Each extension adds a
first-class editing experience — dynamic dropdowns, custom captions, context commands — for
one or more GeneXus patterns.

Each extension's `.vsix` is published as a **GitHub Release** of this repository (see the
[Releases](../../releases) page). Each `extensions/<name>/` folder holds its README + CHANGELOG.

## Available extensions

| Extension | Provider | Patterns | Download | Docs |
|---|---|---|---|---|
| **GeneXus Work With** | KBBridge | Work With (Web) | [⬇ Releases](../../releases) | [README](extensions/genexus-workwith/README.md) · [CHANGELOG](extensions/genexus-workwith/CHANGELOG.md) |
| **PXTools Patterns** | PuntoExe | PXWorkWith, PXParameterRequest, PXComposer, and more | [⬇ Releases](../../releases) | [README](extensions/pxtools-patterns/README.md) · [CHANGELOG](extensions/pxtools-patterns/CHANGELOG.md) |

## Installing a pattern extension

1. Make sure **KB Editor** (`kbbridge.genexus-visual-editor`) is installed.
2. Download the extension's `.vsix` from its Release.
3. In VS Code / VSCodium: **Extensions ▸ … ▸ Install from VSIX…** (or
   `code --install-extension <file>.vsix`).
4. **Reload Window**, then open a `.gxPattern` instance of a supported pattern.

## Maintainership

This catalog is **curated solely by KBBridge** — it only distributes the `.vsix` releases and
their listings. External pull requests are not accepted. To **suggest** a pattern extension
for listing, or to **report a problem**, please [open an Issue](../../issues).

## Building a pattern extension

New to this? Start with the **Pattern Extensibility for KB Editor** documentation and the
`kbbridge-editor-pattern-starter` template.
