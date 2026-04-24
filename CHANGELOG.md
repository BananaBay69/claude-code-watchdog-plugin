# Changelog

## v0.1.0 — 2026-04-24

Minimum CLI version: **v0.1.3** (earlier versions either lack the sidecar
config path or have the `curl | bash` install bug).

### Added
- SessionStart hook (`check-cli.sh`) that auto-installs the CLI when missing and version-checks it when present.
- UserPromptSubmit + Stop hooks (`heartbeat.sh`) that write the v1 heartbeat format atomically, honouring the sidecar `config.env` for custom paths.
- Four slash commands: `install`, `status`, `update`, `uninstall`.
- CI: shellcheck + smoke tests.
