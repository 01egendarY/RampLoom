# Controls and settings

All controls can be rebound in Minecraft's Controls menu under **RampLoom**.

| Default | Action |
|---|---|
| 1 / 2 / 3 / 4 | Wall / floor / ramp / roof |
| Left mouse | Place immediately; hold for continuous building |
| Middle mouse / H | Rotate |
| Right mouse | Cycle wood / stone / metal |
| G | Enter editing / confirm |
| Left mouse while editing | Select cells |
| Right mouse while editing | Reset draft |
| Mouse wheel while editing | Reset to the purchased shape and confirm |
| F | Repair one health stage for one resource |
| U | Upgrade wood → stone → metal |
| Z | Cycle 3×3 / 3×1 / 3×2; enlarge purchased width while editing |
| B | Toggle building and the normal hotbar |
| J | Show / hide instructions |
| Mouse wheel outside editing / 5–9 | Return to the normal hotbar |

The first placement is immediate. Continuous building starts after a configurable
initial delay, default 150 ms, then repeats at most once per server tick.

Open **Esc → RampLoom** for mod settings. No Mod Menu dependency is required.
You can select an interactive mod door or an empty doorway for a vanilla door.
You can also toggle direction stabilization and adjust the first repeat delay.
Placement always uses the shared 3×3 grid; there is no free-placement switch.
English and Russian text follows Minecraft's selected language. Keyboard letters
in the HUD follow physical bindings rather than the Windows keyboard layout.

## Grid placement

Walls snap to the four boundaries of the player's cell. Turn and place to build
a box; looking upward selects an upper level. Floors and ramps can use the current
or neighboring cell, including landings and the next upward flight. Looking to
the side of a ramp selects a side cell instead of forcing an upward continuation.

For narrow pieces, aim at the desired strip inside the cell: any one of three
strips for 3×1 or either adjacent pair for 3×2. The quiet outline shows the full
cell. Only one piece of each kind can occupy its slot, even if edited or narrow.
Adjacent cells share their common wall boundary, so a second wall cannot stack there.

## Editing and expansion

Press **G** while aiming at a piece. Walls, floors and ramps have a 3×3 edit canvas;
roofs use corner controls. Left-click cells to remove or restore portions, then
press **G** to confirm. Ramps accept connected straight, L and U patterns.

Adding cells outside the purchased strips expands the envelope and shows the
additional material cost. **Z** also enlarges purchased width while editing.
Adding one strip costs **2** units; expanding 3×1 directly to 3×3 costs **3**.
Reaching across a missing middle strip purchases that intervening strip too.

Shrinking the visible shape does not reduce the purchased size or refund materials.
Right-click resets the draft to the whole purchased shape; the mouse wheel resets
and confirms immediately. For example, a piece expanded to 3×3 always resets to
3×3, even after a later edit leaves only one strip visible.

## Materials

Wood uses planks, stone uses cobblestone and metal uses iron ingots. Every piece
has three mining stages; appropriate axes/pickaxes affect mining speed. The
complete geometry remains until the final stage is destroyed.
