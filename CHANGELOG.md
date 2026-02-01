# Changelog

All notable changes to the RiskVoid Security Linter extension will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.0.2] - 2026-01-14

### Fixed

- **Critical**: Fixed extension activation failure on fresh installs from VSCode Marketplace
  - Migrated from native tree-sitter to web-tree-sitter (WASM-based)
  - Full AST parsing now works on all platforms without native compilation
  - WASM files bundled with extension for reliable cross-platform support
  - Intelligence layer (context-aware analysis, threat modeling) fully functional

## [0.0.1] - 2026-01-11

### Added

#### Security Analysis

- Real-time vulnerability detection as you code
- OWASP Top 10 coverage out of the box
- Support for JavaScript, TypeScript, Python, and Java
- Detection of SQL injection, XSS, command injection, and more
- Hardcoded secrets and credential detection
- Weak cryptography identification

#### Smart Prioritization

- Context-aware risk scoring
- Automatic identification of critical code paths
- Business impact-based prioritization
- Configurable criticality via `.riskvoid.yml` files

#### Supply Chain Security

- Dependency vulnerability scanning
- CVE details with severity scores
- Fix recommendations with version guidance
- Support for npm and pip packages

#### User Interface

- Interactive dashboard with tabbed interface
- Real-time security score (0-100) in status bar
- Clickable issues for direct code navigation
- Detailed hover cards with explanations
- Color-coded severity indicators

#### Commands

- Scan Current File
- Scan Workspace
- Scan Dependencies
- Show Security Report
- Clear Dependency Cache

#### Configuration

- 40+ configurable settings
- Performance tuning options
- UI customization
- Criticality path configuration

### Privacy

- 100% local code analysis
- No source code upload
- No telemetry or tracking

---

[0.0.2]: https://github.com/riskvoid/riskvoid-vscode/releases/tag/v0.0.2
[0.0.1]: https://github.com/riskvoid/riskvoid-vscode/releases/tag/v0.0.1
