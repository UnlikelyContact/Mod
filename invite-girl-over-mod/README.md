# Sapphic Girlfriends

A relationship mod for X-Change Life that adds lesbian encounters, girlfriend mechanics, and female-female bar pickup features.

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
- **Position selection menus with varying energy costs** (like male player scenes):
  - **Passive (being pleasured):**
    - Slow and sensual (free) - gentle licking positions
    - Let her have her way (free) - random position
    - Beg for more (1⚡) - intense fingering positions
    - Edge yourself (1⚡) - try to hold back
  - **Active (pleasuring her):**
    - Go down on her gently (free) - gentle oral
    - Pleasure her (free) - random position
    - Tongue and fingers (1⚡) - skilled combo techniques
    - Make her scream (2⚡⚡) - intense positions, harder quicktime
  - **Combined positions:**
    - 69 together (1⚡) - mutual pleasure
    - Scissor slow (1⚡) - standard tribbing
    - Scissor intense (2⚡⚡) - aggressive grinding, harder quicktime
- **Fitness-based stamina system:** High fitness (8+) reduces energy costs by 1
- **NPC arousal system:** Build arousal through kissing and foreplay to unlock intense options
- **Trait-specific bonuses:**
  - Slut NPCs: Start at high arousal, easier to please
  - Shy NPCs: Start at low arousal, intense options locked until aroused
  - Athletic NPCs: Additional stamina cost reduction
- **Mutual orgasm bonus:** Special scene when both climax together
- **Post-sex options:** Cuddle, pillow talk, or go again
- Uses existing ff media from the game (Jia/Callie workout scenes)
- Trait-based dialogue for lesbian encounters
- Different quicktime difficulties and pleasure gains based on position intensity

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
- **Passive positions (8 videos):**
  - 20 passive yoga block, 21 passive pile licker, 22 passive upside down fingering
  - 23 passive slow licking, 24 passive fingering from behind, 25 passive fast fingering
  - 26 passive licking lips, 27 passive pussy sucking
- **Active positions (7 videos):**
  - 30 active going down, 31 active circular licking, 32 active tongue and fingers
  - 33 active clit focus, 34 active fingering, 35 active up and down, 36 active fast double action
- **Combined positions:**
  - 28 passive 69 (base game's actual 69 video)
  - Scissors: Uses 35/36 as substitutes (no dedicated scissors video in base game)

## Compatibility

- Requires X-Change Life version 0.17f or later
- Overrides the `refresh possible activities relationships` passage
- Overrides the `bar chat girl options female` passage
- Hooks into `[girl_number]` passage tag (non-override, adds girlfriend tag)
- Compatible with other mods that add bar girls (uses dynamic detection)

## Changelog

### v1.5.0
- **Fitness-based stamina system:**
  - Players with fitness 8+ get 1⚡ discount on all position costs
  - Athletic NPCs provide additional stamina bonus
  - Minimum cost is always 0 (free positions stay free)
- **NPC arousal system:**
  - NPCs have arousal level (0-5) that builds during the scene
  - Kissing increases arousal by 1
  - Arousal affects dialogue ("She's getting into it...", "She's desperate for release...")
  - High arousal (3+) unlocks intense options for shy NPCs
  - Higher arousal = more pleasure gain per action
- **Trait-specific bonuses:**
  - **Slut:** Starts at arousal 3, +2 arousal bonus throughout
  - **Shy:** Starts at arousal 0, intense options locked until arousal reaches 3
  - **Athletic:** Extra stamina cost reduction (stacks with player fitness)
- **Mutual orgasm bonus:**
  - If both player and NPC are near climax (80%+ pleasure), triggers special scene
  - Bonus relationship gains (+2 attraction, +2 friendship)
  - Unique dialogue celebrating the shared moment
- **Post-sex options:**
  - **Cuddle:** Relaxing afterglow (+1 friendship, small energy recovery)
  - **Pillow talk:** Deepen connection (+2 friendship, +1 attraction)
  - **Go again:** Start another round (if stamina permits)
- Arousal-based dialogue throughout all menus
- Updated code comments documenting all new systems

### v1.4.0
- **Added position selection menus with energy costs for lesbian sex scenes**
  - Passive positions: slow and sensual (free), let her have her way (free), beg for more (1⚡), edge yourself (1⚡)
  - Active positions: go down gently (free), pleasure her (free), tongue and fingers (1⚡), make her scream (2⚡⚡)
  - Scissor positions: slow (1⚡), intense (2⚡⚡)
- Different quicktime difficulties and pleasure gains based on position intensity
- **Fixed media path bugs:**
  - "27 passive sucking.mp4" → "27 passive pussy sucking.mp4"
  - "37 active 69.mp4" → "28 passive 69.mp4" (correct base game path)
  - "38 scissors.mp4" → Uses 35/36 active videos (scissors video doesn't exist in base game)
- Added dedicated result passages for each intensity level
- Video selection now matches intensity choice (gentle positions use slower videos, intense uses faster videos)
- Added extensive code comments for easier modification by other modders

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
