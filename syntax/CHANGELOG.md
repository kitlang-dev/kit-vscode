# Change Log

All notable changes to the "kitlang" extension will be documented in this file.

## [0.1.0] — 2026-08-09

### Added
- Comprehensive syntax highlighting for all Kit keywords and constructs.
- Grammar unit tests covering keywords, operators, numbers, strings, types, comments, and preprocessor syntax.
- Test infrastructure using `vscode-tmgrammar-test`.
- `pnpm-workspace.yaml` for pnpm 11 build-script approval.
- Language configuration with `autoClosingPairs`, indentation rules, and `onEnterRules`.
- `.vscodeignore` for proper VSIX packaging.

### Changed
- Minimum VS Code engine requirement: `^1.25.0` → `^1.80.0`.
- Grammar source format retained as `kit.YAML-tmLanguage`; build generates `kit.tmLanguage.json`.
- Build system migrated from npm to pnpm for deterministic dependency management.
- Updated `devDependencies`: `@vscode/vsce`, `js-yaml`, and `vscode-tmgrammar-test`.

### Fixed
- Hex numeric literals now support uppercase hex digits (`0xFF`, `0xDEAD_BEEF`).
- `::` (cons operator) correctly scoped as `keyword.operator.cons.kit` before `:`.
- `...` (ellipsis) operator no longer fails at line start.
- `@identifier` correctly scoped before custom operator catch-all.
- Removed stale `[]()` references in grammar comments.

### Removed
- Vendored third-party themes (`themes/` directory).
- Legacy plist grammar (`syntaxes/kit.tmLanguage`).
- Outdated `.npmrc` config (not supported by pnpm 11).
