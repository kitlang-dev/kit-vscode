# kit-vscode

This repository hosts VSCode tooling for the [Kit programming
language](https://kitlang.dev/). This project is a fork of
[AlexPoulsen/kit-vscode](https://github.com/AlexPoulsen/kit-vscode).

It contains a few independent extensions, each published under its own ID and
license:

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

Each extension is built and tested independently by CI (see
[`ci.yml`](./.github/workflows/ci.yml)), which runs a matrix over both
`syntax/` and `language-server/`. To build locally, see each extension's own
README.

## License

This repository is [REUSE](https://reuse.software)-compliant; license texts live
in [`LICENSES/`](./LICENSES) and per-file declarations are in
[`REUSE.toml`](./REUSE.toml). Each extension carries its own `LICENSE` file
(symlinked to `LICENSES/<SPDX>.txt`) so `vsce` packages it as `LICENSE.txt`.

- [`language-server`](./language-server): **MIT** (see
  [`language-server/LICENSE`](./language-server/LICENSE)).
- [`syntax`](./syntax): **LGPL-3.0** (see [`syntax/LICENSE`](syntax/LICENSE)).
