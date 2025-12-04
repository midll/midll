# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

## [0.3.0] - 2025-12-04
### Added
- `record` type for nested objects/structures.
- Typed array syntax `array[type]` for explicit array typing (e.g., `array[record]`, `array[string]`).
- Support for arrays of records with braces syntax.
- Multiple examples showing single vs. multiple records patterns.

### Changed
- Updated example config to demonstrate `record` type usage.
- Refactored `mandate` section to use `array[record]` with proper dependency structure.
- Improved example file with clarifying comments for author field patterns.

### Fixed
- Corrected version field typing from `int` to `string` in dependency examples.

## [0.2.0] - 2025-12-03
### Added
- Support for both brace-based and indentation-based sections in ABNF and EBNF grammars.
- Updated example config to use indentation-based sub-objects.

### Changed
- Dropped ANTLR grammar due to complexity of indentation handling and custom lexer requirements.
- Project now focuses on ABNF and EBNF grammars for specification and parsing.

## [0.1.0] - 2025-12-2
### Added
- Initial project structure and documentation.
- ABNF and EBNF grammars for Midll configuration language.
- Example configuration file.
