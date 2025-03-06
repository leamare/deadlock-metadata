# Simon-Deadlock-Metadata

Metadata for Valve's game Deadlock (aka Project8, Citadel, Neon Prime, Shadowline), used for LRG/Simon related projects.

The metadata is generated based on the game files, SteamDB metadata and localization files.

## Available files

- Heroes metadata
  - `heroes`
    - `base`
      - `status` reflects hero's availability: enum ["available", "labs", "in_devel", "notahero"]
    - `stats` lists all relevant hero stats, inspired by the sheet made by lamarrite
    - `names` lists hero names in all available languages
    - `abilities` - abilities of heroes
- Items
  - `items`
    - `base` has a map of item IDs (MurmurHash2) to item tags
    - `names` lists item names in all available languages
    - `stats` lists all the main stats parameters for every item
- `patchdates` - dates and tags for the game's updates
  - It also includes version from earlier stages of development and groups them together, though anything before the original playtest date is unknown. Many updates were filtered out, leaving only one update per 15 hours (or when it's most likely that there were no significant changes in this time window).
  - All versions have tags, marking notable changes in the game or development stages (though precise dates and the size of the pre-deadlock updates are unknown). What patch relates to what development stage was decided based on various reports about the game, leaks and drops/spikes in patch rate activity.
  - This file aims to be the same as Dota 2 counterpart in Dota metadata repo. Thus every major update is treated as a separate "patch version" and every minor patch is treated as a "letter patch".

## TODO:

- `abilities/base`
- `abilities/names`
- `colors` ??