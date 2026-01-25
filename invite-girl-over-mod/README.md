# Invite Girl Over Mod

A mod for X-Change Life that allows players to invite girlfriends over in the evening, mirroring the "Invite guy over" feature. Works for both male and female players.

## Features

### For Male Players
- Adds "Invite girl over" as an evening activity
- Bar girls automatically become girlfriends when you get their number
- Full sex scene integration with bar girls (uses game's media assets)
- Trait-based dialogue (slut, bimbo, religious, assertive, etc.)
- Option for her to stay the night

### For Female Players (Lesbian Content)
- Same "Invite girl over" activity when playing as female
- Dedicated female-female sex scenes with video/image media
- Multiple position options (passive, active, 69)
- Uses existing ff media from the game (Jia/Callie workout scenes)
- Trait-based dialogue for lesbian encounters

### Lesbian Bar Pickup
- Override for `bar chat girl options female` passage
- Female players can flirt with women at the bar
- Pickup lines, buy drinks, ask for number, ask to hook up
- Full integration with ff sex scenes
- Girls automatically become girlfriends after hooking up

### General
- Track relationships with girls who become "girlfriends"
- Relationship progression (friendship, attraction)
- Dynamic bar girl detection (works with modded bar girls)

## Installation

1. Copy the `invite_girl_over.twee` and `invite_girl_over.meta` files to your mods folder
2. The mod will automatically integrate with the game's activity system

## How It Works

The mod adds a "girlfriend" relationship tag system. When you build relationships with female NPCs and they become interested in you, they can become girlfriends.

The "Invite girl over" option appears in evening activities when:
- You have at least one girlfriend in your relationships
- Works for both male AND female player characters

## Media Used

### Male Player (with bar girls)
- Uses existing bar girl media: `npc/girls/{id}/strip/`, `npc/girls/{id}/sex/`

### Female Player (lesbian scenes)
- Uses Jia workout ff media: `scenes/characters/jia/sex/workout/ff/`
- Positions include: active going down, circular licking, tongue and fingers, clit focus, fingering, 69

## Compatibility

- Requires X-Change Life version 0.17f or later
- Overrides the `refresh possible activities relationships` passage
- Overrides the `bar chat girl options female` passage
- Hooks into `[girl_number]` passage tag (non-override, adds girlfriend tag)
- Compatible with other mods that add bar girls (uses dynamic detection)

## Changelog

### v1.3.0
- Fixed attraction check error (was checking NPC directly instead of relationships)
- Added `[girl_number]` passage tag hook for male players
- Bar girls now automatically become girlfriends when males get their number
- Improved lesbian bar options to match game patterns (boredom checks, event tracking)
- Fixed duplicate option issues in lesbian bar pickup

### v1.2.0
- Added lesbian bar pickup for female players
- Override for `bar chat girl options female` passage
- Pickup lines, buying drinks, asking for number, asking to hook up
- Full bar-to-bedroom flow for lesbian encounters
- Girls from bar become girlfriends automatically

### v1.1.0
- Added lesbian hookup support for female players
- Integrated ff media from game assets
- Multiple position options for lesbian scenes
- Trait-based dialogue for both straight and lesbian encounters

### v1.0.0
- Initial release
- Male player can invite girlfriends over
- Integration with bar girl sex system

## Files

- `invite_girl_over.twee` - Main mod content
- `invite_girl_over.meta` - Mod metadata
- `README.md` - This file
