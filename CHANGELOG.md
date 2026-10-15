# Changelog

## 0.5.2 — 2026-10-14

### Changed
- Adopt RampLoom as the public name, including English/Russian settings labels.
- Add original painted branding and an embedded Fabric icon.
- Specify free binary use, server use and unmodified modpack distribution.
- Preserve the internal mod ID, saved data and 0.5.1 gameplay mechanics.

## 0.5.1 — 2026-10-12

### Fixed
- Prevent a crash when loading saved building chunks during a support audit.
- Retry audits invalidated by chunk callbacks and delay collapse until the graph
  is complete and current.

## 0.5.0 — 2026-10-12

### Added
- Configurable initial continuous-building delay.
- Material upgrades and settings for a door or empty doorway.
- Explicit English and Russian localization.

### Fixed
- Reject overlapping floors across rotations, materials and edited shapes.
- Improve first-piece placement on Minecraft's block grid and attachments at
  ramp, terrain and leaf edges.
