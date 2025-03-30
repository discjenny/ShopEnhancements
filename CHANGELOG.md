# Changelog

All notable changes to this project will be documented in this file.

# Changelog

## [2.0.0] - 03-29-2025

### Added
- Expanded shop space using GalaxyMods' custom shelf prefab
- Global price multiplier (0.1x to 5.0x) for all shop items
- Individual maximum counts for each upgrade type:
  - Health Upgrades
  - Energy Upgrades
  - Strength Upgrades
  - Speed Upgrades
  - Jump Upgrades
  - Map Upgrades
  - Launch Upgrades
  - Range Upgrades
- Configurable min/max counts for new item categories:
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
- New upgrade cost scaling mode: HighestPlayer
  - Cost scales with highest level any player has for that upgrade
  - Alternative to vanilla's total-purchased scaling

### Changed
- Completely reworked shop item spawning system
- Improved configuration organization with three distinct sections:
  - Shop Settings - Item Count
  - Shop Settings - Cost Scaling
  - Upgrade Settings - Max Amount
- Better logging for debugging and troubleshooting
- Updated to use REPOLib for core functionality

### Fixed
- Item spawning issues in multiplayer
- Upgrade cost scaling inconsistencies
- Various edge cases with item counts

## [1.0.0] - Initial Release

- Basic shop enhancements
- Configurable upgrade item counts
- Initial multiplayer support 

## [1.1.0] - 03-29-2025

### Added
*   New configuration option `UpgradeCostScalingMode` with two modes:
    * `Vanilla`: Preserves default game behavior (50% price increase per purchase, 5% discount per additional player)
    * `HighestPlayer`: Price scales only with highest upgrade level among players, ignoring multi-player discounts
*   Automatic cleanup of outdated configuration entries during updates
*   Better organization of configuration file into clear sections

### Changed
*   Improved configuration handling to preserve user settings during updates
*   Reorganized configuration file into logical sections for better readability

## [1.0.0] - 03-29-2025

### Added

*   Initial release.
*   Configuration option `MaxUpgradeItems` to set the maximum number of shop upgrades (default: 14, range: 0-14).
*   Configuration option `MinUpgradeItems` to set the minimum number of shop upgrades (default: 14, range: 0-14).
*   Validation to ensure MinUpgradeItems is not greater than MaxUpgradeItems.
*   Randomization of the number of upgrade items spawned between the configured (and validated) min and max values each time the shop initializes.
*   Functionality applies only when the player is the host (MasterClient) or in singleplayer mode. 