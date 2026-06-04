# Dragon Addon for Minecraft Bedrock Edition

## Overview
This addon adds **4 unique, rideable dragon variants** to Minecraft Bedrock Edition 1.21+:

- **Fire Dragon** (Red/Orange) - Aggressive, attacks with fire breath
- **Ice Dragon** (Blue/White) - Calm, peaceful variant
- **Forest Dragon** (Green) - Rare, protective behavior
- **Sky Dragon** (Purple/White) - Neutral, uses wind effects

## Features

✅ **Tameable & Rideable**
- Tame dragons by feeding them **raw fish**
- Ride tamed dragons with full flight control (WASD + Space)
- Dragons follow the player when tamed

✅ **Growth Stages**
- Baby → Adolescent → Adult
- Dragons grow through feeding with raw fish
- Health and stats increase with each stage

✅ **Unique Behaviors**
- Fire Dragon: Aggressive, attacks with fire
- Ice Dragon: Calm, no attacks
- Forest Dragon: Protective of players
- Sky Dragon: Neutral, uses wind effects

✅ **Natural Spawning**
- Fire Dragons spawn in nether biomes (night)
- Ice Dragons spawn in snowy biomes
- Forest Dragons spawn in forest biomes (rare)
- Sky Dragons spawn in mountain biomes (day)

✅ **Summoning**
- Create dragon eggs via commands
- Summon specific dragon variants

## Installation

### PC & Mobile

1. **Download** both packs from the repository
2. Copy to your Minecraft packs folder:
   - Windows: `%appdata%\.minecraft\development_packs\`
   - Android: `/sdcard/Android/data/com.mojang.minecraftpe/files/games/com.mojang/development_packs/`
   - iOS: Check the File app → Minecraft folder
3. Enable both packs in world settings (Behavior + Resource Pack)
4. Create a new world with these packs enabled

## Commands

### Summon Dragon Egg
```
/give @s dragon_egg
```

### Summon Dragon Directly
```
/summon dragon:fire_dragon ~ ~1 ~
/summon dragon:ice_dragon ~ ~1 ~
/summon dragon:forest_dragon ~ ~1 ~
/summon dragon:sky_dragon ~ ~1 ~
```

### Trigger Growth Event
```
/execute @e[type=dragon:fire_dragon,tag=baby] ~~~ event entity @s dragon:grow_to_adolescent
```

## Taming & Riding

1. **Find a Dragon** - Look for them spawning naturally or summon them
2. **Feed Raw Fish** - Right-click/interact with the dragon while holding raw fish
3. **Wait for Hearts** - Once tamed (hearts appear), you can ride it
4. **Mount & Control**:
   - Sneak + Right-click to mount
   - WASD to move/fly
   - Space to ascend
   - Shift to descend
   - Mouse to look around

## Growth Progression

| Stage | Health | Scale | Speed |
|-------|--------|-------|-------|
| Baby | 10-13 | 0.5x | Slow |
| Adolescent | 20-26 | 0.75x | Medium |
| Adult | 40-48 | 1.0x | Fast |

## Loot Drops

- **Dragon Scale** (2-4 per dragon)
- **Raw Fish** (Fire Dragon only, 1-2)

## Biome Spawning

| Dragon | Biome | Condition |
|--------|-------|-----------|
| Fire | Nether | Night (low light) |
| Ice | Snow | Any time |
| Forest | Forest | Night (rare, 4 weight) |
| Sky | Mountain | Day (high light) |

## Technical Details

- **Format Version**: 1.20.0+
- **Min Engine Version**: 1.21.0
- **Fully Compatible**: Bedrock Edition (Mobile, Console, Windows)
- **No Java Edition Support**

## Troubleshooting

**Dragons not spawning?**
- Check difficulty is not peaceful
- Ensure you're in the correct biome
- Make sure both packs are enabled

**Can't tame dragon?**
- Use raw fish, not other items
- Try right-clicking multiple times
- Ensure you're not in creative mode

**Rider issues?**
- Make sure you're on an adult or adolescent dragon
- Check that the rideable component is enabled
- Try mounting again after waiting a moment

## Future Updates

Planned features (v2.0):
- Dragon armor customization
- More particle effects
- Additional abilities per variant
- Breeding system improvements

## Credits

Created for Minecraft Bedrock Edition as a professional addon.

---

**Questions?** Check the entity files in `behavior_packs/dragon_addon/entities/` for detailed configurations.
