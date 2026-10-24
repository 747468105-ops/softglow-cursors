# Cursor Coverage

Trial 0.3. Both palettes use the same state mapping. Not a complete release.

## Implemented

- Arrow / ArrowS.
- Text / IBeamS / IBeamXOR.
- Link / Pointing.
- Open / Closed hand.
- Wait / Busy: 24 frames, 0.08 seconds per frame.
- Horizontal resize: cursor IDs 17, 18, 19, 27, 28, 38.
- Vertical resize: cursor IDs 21, 22, 23, 31, 32, 36.
- NE/SW diagonal: cursor IDs 29, 30, 37.
- NW/SE diagonal: cursor IDs 33, 34, 35.

Directional edges currently share the double-ended artwork for their axis;
separate one-sided edge artwork is a future refinement, not a missing mapping.

## Missing Compared With Bibata Modern Ice

- Alias / Copy / Copy Drag.
- Move.
- Context arrow / Context menu.
- Forbidden / Help / Poof.
- Precision crosshair / Crosshair 2 / Cell.
- Horizontal text.

## Additional System Slots

- Screenshot camera / camera variants.
- Counting hand states.
- Cell XOR / Resize Square.
- Zoom In / Zoom Out.

Unimplemented roles are intentionally not filled with another theme's artwork.
App-drawn pointers may remain unchanged even after all system slots are covered.

## References

- MaCursor: CursorEngine/MACCursorDefinitions.swift (cursorMap / browserAliasMap).
- Official MaCursor theme bundle: BibataModernIce.cursor (39 visible roles).
