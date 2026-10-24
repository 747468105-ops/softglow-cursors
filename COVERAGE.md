# Cursor Coverage

## 中文覆盖清单

当前为 v0.3 试用版，蓝色和烟灰色使用相同的状态映射，不是完整发布版。

已做：普通箭头、文字选择、链接/指向手形、张手、握手、横向/纵向缩放、东北-西南和西北-东南两个斜向缩放、等待和忙碌动画。

窗口边缘暂时共用所在轴向的双向箭头，尚未单独绘制单向边缘图形。

待补齐：复制、别名、拖拽复制、移动、上下文菜单、禁止、帮助、移除特效、十字准星、单元格选择、横排文字光标。

其他系统场景还包括：截图相机、计数手形、异或单元格、方形缩放、放大和缩小。

没有实现的状态不拼接第三方主题图案。即使补齐系统状态，一些应用自己绘制的指针仍可能不变。

下方为英文技术清单，保留标识方便开发者检查。

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
