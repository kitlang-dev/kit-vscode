# Kit language support for Visual Studio Code

Syntax highlighting and language support for the [Kit programming language](https://kitlang.dev/).

## Features

- Full syntax highlighting for Kit source files (`.kit`).
- Block comments, inline C blocks, character literals, and backtick identifiers.
- Support for Kit-specific constructs: `trait`, `implement`, `rule`/`rules`, `specialise`, `rewrite`, etc.

## LSP Support

A Language Server Protocol implementation is **coming soon**.

## Installation

### From VS Code Marketplace
Search for "Kit" in the Extensions view (`Ctrl+Shift+X`).

### From VSIX
```bash
pnpm run package
code --install-extension *.vsix
```

## Development

```bash
pnpm install
pnpm run build        # generate JSON grammar from YAML source
pnpm test             # run grammar unit tests
```

## License

LGPL-3.0. The full license text is in [`LICENSE`](./LICENSE) in this folder.
