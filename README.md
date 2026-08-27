# kit-vscode

This repository hosts the official VSCode tooling for the
[Kit programming language](https://kitlang.dev/). It contains a few independent
extensions, each published under its own ID and license:

| Extension | ID | Path |
|-----------|---------------|------|
| Syntax | `kitlang.syntax` | [`syntax/`](./syntax) |
| LSP | `kitlang.lsp` | [`language-server/`](./language-server) |

## Extensions

### Kit Syntax (`kitlang.syntax`)

Syntax highlighting for Kit.

### Kit LSP (`kitlang.lsp`)

Language server support for Kit. Currently a placeholder that contributes sample
configuration options only.

## Building

Each extension is built and tested independently by CI
(see [`.github/workflows/ci.yml`](./.github/workflows/ci.yml)), which runs a
matrix over both `syntax/` and `language-server/`. To build locally, see each
extension's own README.

## License

This repository intentionally has no single root license; each extension carries
its own `LICENSE` file in its folder.

- [`language-server`](./language-server): **MIT** (see [`language-server/LICENSE`](./language-server/LICENSE)).
- [`syntax`](./syntax): **LGPL-3.0** (see [`syntax/LICENSE`](syntax/LICENSE)).
