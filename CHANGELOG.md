# Changelog

All notable changes to this ZMK firmware configuration will be documented in this file.

## [Unreleased]

## [2026-03-05] - Workflow Version Fix

### Changed
- Pinned GitHub Actions workflow to ZMK `v0.3` tag instead of `main`
- Fixes build failures caused by new Zephyr 4.1 compatibility check in ZMK main branch

### Added
- CHANGELOG.md for tracking firmware changes and build history

## [2025-02-XX] - Settings Reset

### Added
- `settings_reset` shield to build.yaml for Bluetooth bond clearing utility

## [2025-02-XX] - Keymap Reorganization

### Changed
- Fixed keymap key order
- Remapped keymap for components-down nice!nano mounting
- Removed overlay files in favor of firmware file swapping

---

## Build Workflow

When changes are pushed to `main`, GitHub Actions automatically:
1. Builds firmware for left and right halves
2. Generates `settings_reset` utility
3. Produces downloadable `firmware.zip` artifact

## Version Format

Dates are used as version identifiers: `[YYYY-MM-DD]`
