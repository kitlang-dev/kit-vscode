# kit-vscode

This repository hosts the official VSCode tooling for the
[Kit programming language](https://kitlang.org/). It contains two independent
extensions, each published under its own marketplace ID and license:

| Extension | Marketplace ID | Path | License |
|-----------|---------------|------|---------|
| Kit Syntax | `kitlang.syntax` | [`syntax/`](./syntax) | LGPL-3.0 (see [`LICENSE`](./LICENSE)) |
| Kit LSP | `kitlang.lsp` | [`language-server/`](./language-server) | MIT (see [`language-server/LICENSE`](./language-server/LICENSE)) |

## Extensions

### Kit Syntax (`kitlang.syntax`)
Syntax highlighting for Kit. Licensed under **LGPL-3.0**; the license text is the
repository-root [`LICENSE`](./LICENSE), symlinked into `syntax/LICENSE`.

### Kit LSP (`kitlang.lsp`)
Language server support for Kit. Currently a placeholder that contributes sample
configuration options only. Licensed under **MIT**; see
[`language-server/LICENSE`](./language-server/LICENSE).

## Building

Each extension is built and tested independently by CI
(see [`.github/workflows/ci.yml`](./.github/workflows/ci.yml)), which runs a
matrix over both `syntax/` and `language-server/`. To build locally, see each
extension's own README.
