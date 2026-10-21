# Changelog

## 0.6.2 — 2026-10-21

Changes since the previous public release, 0.5.2. Versions 0.6.0 and 0.6.1 were
local development builds, not separate public releases.

### Added

- Shared 3×3 placement cells, with four wall boundaries around the player's cell,
  side ramps and upper landings.
- Aim-based strip placement: choose any single strip for 3×1 or either neighboring
  pair for 3×2 without moving the shared cell.
- Editor expansion for materials: 3×1 → 3×2 costs 2, 3×1 → 3×3 costs 3,
  and 3×2 → 3×3 costs 2 units of the piece's material.
- Persistent purchased size and strip positions, independent of the visible edit.
  Shape resets restore the purchased envelope without charging again.
- Optional direction stabilization to reduce accidental turns near cell edges.

### Changed

- New placement sizes are 3×3, 3×1 and 3×2. Saved 2×2 and 2×1 pieces remain readable.
- Reserve one floor, ramp or roof slot per cell and level, even after narrowing,
  rotation or editing. Walls occupy separate boundary slots shared by adjacent cells.
- Walls, floors and ramps use a full 3×3 editing canvas; roofs retain corner editing.
- Existing saved structures retain their positions and legacy editing behavior.
- Require matching updated client/server versions for the new placement protocol.

### Fixed

- Selecting all nine cells now expands narrow walls, floors and ramps to full size
  in one confirmation.
- Centered single strips expand equally to either side; bought positions survive resets and reloads.
- Complete separated ramp strips connect through the middle; valid routes no longer
  depend on the former starting cell.
- Remove texture flicker at mixed-material wall/floor intersections.
- Preserve water rendering beneath placement/edit previews and temporary building
  effects, with opaque blocks still hiding the preview normally.

### Removed

- The free/grid placement switch. Placement always uses the shared 3×3 grid;
  old saved free-placement preferences no longer enable the previous mode.
- Two-block sizes from the new-placement cycle.

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
