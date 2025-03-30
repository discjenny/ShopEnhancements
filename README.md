# Shop Enhancements

A mod that enhances the shop experience in Lethal Company by adding more shelf space, configurable item counts, and price scaling options.

## Features

### 🛍️ Expanded Shop Space
- Additional shelf space using GalaxyMods' custom shelf prefab (Credit: [GalaxyMods](https://github.com/InfusedGalaxy))
- Better organization of items in the shop
- More room for the increased item variety

### 📦 Configurable Item Counts
Control the minimum and maximum number of items that can appear in the shop for each category:
- Regular Carts
- Pocket Carts
- Guns
- Melee Weapons
- Grenades
- Drones
- Mines
- Trackers
- Power Crystals
- Health Packs
- Upgrades

### 💰 Price Scaling Options
- Global Price Multiplier: Adjust all shop prices with a single multiplier (0.1x to 5.0x)
- Upgrade Cost Scaling Modes:
  - Vanilla: Base game behavior (cost scales with total purchased)
  - HighestPlayer: Cost scales with the highest level any single player has for that upgrade

### 🔧 Upgrade Type Controls
Individual maximum counts for each upgrade type:
- Health Upgrades
- Energy Upgrades
- Strength Upgrades
- Speed Upgrades
- Jump Upgrades
- Map Upgrades
- Launch Upgrades
- Range Upgrades

## Configuration

All settings can be found in `BepInEx/config/discjenny.ShopEnhancements.cfg`

The config file is organized into three sections:
1. Shop Settings - Item Count
2. Shop Settings - Cost Scaling
3. Upgrade Settings - Max Amount

### Default Values
- Global Price Multiplier: 1.0 (normal prices)
- Upgrade Cost Mode: Vanilla
- Item Counts: Varies by category, check config file for details
- Upgrade Maximums: Configurable per upgrade type

## Bug Reports

Found a bug? Please report it on our [GitHub Issues page](https://github.com/discjenny/ShopEnhancements/issues).

When reporting bugs, please include:
1. Your mod version
2. Steps to reproduce the issue
3. Expected vs actual behavior
4. Any error messages or logs
5. Whether the issue occurs in single player, as host, or as client

## Credits

- GalaxyMods: Custom shelf prefab used for expanded shop space
- REPOLib: Core dependency providing essential functionality
- Contributors: Everyone who has reported bugs and suggested features