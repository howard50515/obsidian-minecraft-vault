---
id: mine_obsidian_lava_water
type: strategy
auto_generated: true
---

# Mining Obsidian via Lava and Water Casting (Bot-Safe Method)

## Hard Data
* **Spawns/Found/Crafted:** Formed when [[water]] flows over [[lava]] source blocks.
* **Requirements:** [[water_bucket]], [[diamond_pickaxe]] or [[netherite_pickaxe]].
* **Stats/Drops:** Casting [[lava]] with [[water]] creates [[obsidian]] (if the lava is a source block) or [[cobblestone]] (if the lava is flowing).

## The Strategy
To minimize risk, the bot must avoid interaction with flowing liquids. The bot should locate a static, non-flowing [[lava]] pool. Instead of standing in the [[water]] flow—which can cause erratic pathfinding and movement jitter—the bot must stand on a solid block of [[stone]] or [[dirt]] at least ==1== block above the [[lava]] surface.

The bot should place [[water]] from a [[water_bucket]] exactly ==1== block adjacent to the [[lava]] source block to trigger the transformation into [[obsidian]]. Once the [[obsidian]] is formed, the bot should mine it using a [[diamond_pickaxe]] or [[netherite_pickaxe]] from a safe distance. If the bot must descend, it should first place a temporary pillar of [[dirt]] to ensure it has a stable exit path, avoiding any direct contact with [[lava]].

- [ ] Locate a static, non-flowing [[lava]] pool
- [ ] Position on a solid block ==1== block above the [[lava]] surface
- [ ] Place [[water]] adjacent to the [[lava]] source block
- [ ] Mine the created [[obsidian]] using a [[diamond_pickaxe]] or [[netherite_pickaxe]]

> [!danger] CRITICAL WARNING
> Never allow the bot to stand in a [[water]] flow that is directly above [[lava]]. If the [[water]] source is accidentally broken or the bot moves, it may instantly fall into the [[lava]] source, leading to immediate death.

> [!tip] Bot Success Tip
> Use a "safe-anchor" method: place a [[dirt]] block at the bot's feet before interacting with the [[lava]] pool. This prevents the bot from sliding into the [[lava]] due to physics-based movement shifts when interacting with fluids.

*Sources checked:* https://minecraft.wiki/w/Tutorial:Obsidian_farming, https://wikihow.com/Make-Obsidian-in-Minecraft
