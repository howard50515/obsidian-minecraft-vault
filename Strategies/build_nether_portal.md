---
id: build_nether_portal
type: strategy
auto_generated: true
---

# Building a Nether Portal (Bot-Safe Method)

## Hard Data
* **Spawns/Found/Crafted:** Built by placing [[obsidian]] in a vertical rectangular frame.
* **Requirements:** [[obsidian]], [[flint_and_steel]] (or other fire source).
* **Stats/Drops:** Requires a minimum of ==10== [[obsidian]] for a minimal portal (omitting corners) or ==14== [[obsidian]] for a full frame. Internal dimensions must be ==2x3== blocks.

## The Strategy
For an AI bot, the most foolproof method is to construct a full ==4x5== frame including corners to ensure the bot has a stable, predictable boundary for its coordinate-based placement. The bot must first clear a flat ==4x5== area of [[dirt]] or [[stone]] to avoid pathfinding offsets. Once cleared, place the [[obsidian]] in a strict rectangular perimeter.

To activate the portal, the bot should stand at a fixed coordinate adjacent to the interior [[air]] blocks and use [[flint_and_steel]] on the bottom center block. Avoid using [[lava]] as an ignition source, as the bot may struggle to calculate the exact placement required to trigger the portal without contaminating the frame.

- [ ] Clear a flat ==4x5== area of [[stone]] or [[dirt]]
- [ ] Place ==14== blocks of [[obsidian]] to form a full frame (with corners)
- [ ] Position at a fixed coordinate adjacent to the interior
- [ ] Use [[flint_and_steel]] on the bottom center [[obsidian]] block

> [!danger] CRITICAL WARNING
> Do not attempt to "mold" the portal using flowing [[lava]] and [[water]], as the bot's inability to predict fluid flow may lead to [[obsidian]] appearing in incorrect coordinates, causing the bot to get stuck or fall into [[lava]].

> [!tip] Bot Success Tip
> Always build the full frame including corners. This provides the bot with a consistent geometric shape, making it easier to verify the structure via block-scanning before attempting ignition.

*Sources checked:* https://minecraft.wiki/w/Tutorial:Nether_portals, https://minecraft.wiki/w/Nether_Portal_(block)
