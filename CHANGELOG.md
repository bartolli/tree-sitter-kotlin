# Changelog

All notable changes to tree-sitter-kotlin-codanna will be documented in this file.

## [0.4.0] - 2026-11-22

### Changed
- Synced to fwcd/tree-sitter-kotlin `d6af96d` (2026-10-31), 135 commits past the 0.3.9 fork point
- Rust binding exposes `LANGUAGE` (`tree_sitter_language::LanguageFn`); `language()` is removed
- Crate edition 2021; depends on `tree-sitter-language` 0.1 instead of `tree-sitter`

## [0.3.9] - 2025-11-03

### Added
- Fork of tree-sitter-kotlin as tree-sitter-kotlin-codanna for crates.io publication
- FORK-RATIONALE.md documenting temporary fork purpose and migration path
- CLAUDE.md development guide with build commands and architecture overview
- Manual publishing process documentation

### Changed
- Renamed crate from tree-sitter-kotlin to tree-sitter-kotlin-codanna
- Updated repository URL to bartolli/tree-sitter-kotlin
- Disabled deployment workflows (crates.io, npm, GitHub Pages)
- Retained CI workflow for automated testing

### Fixed
- Doctest example using correct crate name tree-sitter-kotlin-codanna

### Notes
This is a temporary fork to enable Codanna to publish to crates.io while upstream 0.3.9 remains unreleased. The fork includes critical fixes from upstream for extension functions, infix operators, fun interfaces, and type parameters with trailing commas. Will migrate back to upstream tree-sitter-kotlin when 0.3.9 is officially published.
