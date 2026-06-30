# GeneXus Work With — for KB Editor

Editor support for the GeneXus **Work With (Web)** pattern inside KB Editor.

- **Provider:** KBBridge
- **Pattern type:** `WorkWith`
- **Requires:** KB Editor (`kbbridge.genexus-visual-editor`)

## What it adds

- **Custom type** — `GridCustomRender` combo editor (settings property `CustomRender`).
- **Caption** — the `Modes` node shows `modes (Insert, Update, …)` listing enabled modes.
- **Custom action** — **"Add Filter Variable…"** on the `FilterAttributes` node.

## Install

1. Install **KB Editor** first.
2. Download `genexus-workwith-kb-editor-<version>.vsix` from the
   [latest Release](../../../releases).
3. **Extensions ▸ … ▸ Install from VSIX…**, then **Reload Window**.
4. Open a Work With `.gxPattern` instance.

## Source & docs

This extension is also the open, worked **reference example** for building KB Editor pattern
extensions (a faithful TypeScript port of the GeneXus Work With pattern). See the
`kbbridge-editor-pattern-genexus-workwith` project and the *Pattern Extensibility for KB
Editor* docs.

## License / attribution

MIT (original TypeScript). Implements the GeneXus Work With pattern's editor behavior; see
the project's `NOTICE.md`. *GeneXus* and *Work With* are trademarks of their respective
owners.
