# Publishing a pattern extension in this catalog

This repository is a **catalog + distribution point** for KB Editor pattern extensions. It
distributes **`.vsix` binaries** via **GitHub Releases**, plus a `README.md` and
`CHANGELOG.md` per extension under `extensions/<ext>/`. It does **not** host extension source
code.

## Steps

1. **Build your `.vsix`** in your own project (`npm run package` / `vsce package`). Make sure
   it declares `"extensionDependencies": ["kbbridge.genexus-visual-editor"]`.
2. **Add a catalog entry**: create `extensions/<your-extension>/` with:
   - `README.md` — description, provider, supported patterns, KB Editor compatibility,
     install instructions, link to the download.
   - `CHANGELOG.md` — version history.
3. **Attach the `.vsix` to a GitHub Release** of this repository (tag `<extension>-vX.Y.Z`)
   so it is downloadable from the Releases page.
4. **Add a row** to the table in the root `README.md`.

## Guidelines

- Only **binaries + docs** belong here — never your extension's source code.
- State the **KB Editor version** your extension was tested against.
- Keep each extension's `CHANGELOG.md` up to date with its releases.
- You retain ownership and licensing of your extension; this catalog only distributes it.
