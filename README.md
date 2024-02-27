# ControlCompany
___
![control_company_banner](https://i.imgur.com/TOW2odr.png)

## Key features
- **Monster Control**: Gain direct control over most monsters, from the tiny **Snare Flea** to the colossal **Forest Keeper**. Each monster comes with its own unique abilities and attributes!
- **Multiplayer**: Yes this works in online multiplayer lobbies! Now go out there and scare your friends!
- **Host only**: Only the host (i.e. you) need to run the mod! This means your friends won't suspect a thing. ;)
- **Ghost Mode**: Stalk your prey before you activate monster mode to find the perfect opportunity to pop out.
- **Nightvision**: While in ghost / monster mode you'll have nightvision enabled.

![forest_giant](https://i.imgur.com/C5NIAcD.gif)

## Available stable monsters (so far)

As of now, the following monsters ([ref](https://www.ign.com/wikis/lethal-company/Lethal_Company_Monsters)) are considered stable. We will continue to update the mod with more stable monsters in the future.
- Baboon Hawk
- Bracken
- Coil-Head
- Company Monster
- Earth Leviathan
- Eyeless Dog
- Forest Keeper
- Hoarding Bug
- Hygrodere (Blob)
- Jester
- Masked
- Nutcracker
- Snare Flea (Centipede)
- Spore Lizard (Puffer)
- Thumper

### Experimental monsters
Experimental monsters are all other monsters in the game files that are not listed above. These monsters are still accessible if you enable the **Extended mode ('0' digit key)** while in Player mode.

Once enabled you will be able to see the full list of monsters to spawn and control for the current level. **These monsters are NOT stable yet so use at your own risk!**

### Modded Monsters
Modded monsters are automatically added as an experimental monster. Some modded monsters may be incompatible and depends if the monster was setup correctly.

## Mod controls
There are 3 player control modes while using the mod, **Player, Ghost and Monster** modes. Control keys can be configured, see [Keybind configuration](#keybind-configuration).

### Player mode
This is just the default player mode as if you were playing the game with a few extra keys.

- **F1 (function key)**: Enter Ghost mode.
- **O key/P key**: Switch the current target. The target is where you will spawn when you enter Ghost mode.

### Ghost mode
This mode lets you roam around the map without being seen. Once you are in this mode you will be able to spawn and control monsters where you are standing.

>  **Mic will be set to push to talk while in this mode**.

- **Function keys**: Depending on the map you'll be able to spawn and control different monsters.
- **O key/P key**: Change the page of available monsters if there are more than 12 possible monsters on the current map.
- **Shift**: Run.
- **Space**: Jump.
- **E**: Open doors.
- **Esc**: Exit Ghost mode and return to Player mode.

### Monster mode
This mode gives you direct control over a monster. [Monsters have unique primary and secondary skills](#monster-abilities).


>  **Mic will be set to push to talk while in this mode**.


- **LMB\***: The monsters primary skill.
- **RMB\***: The monsters secondary skill.
- **F1 (function key)**: Toggle between AI and player-controlled modes.
- **Shift**: Run.
- **E**: Open doors.
- **Left Alt**: Lock enemy rotation.
- **Esc**: Exit the monster mode and return to Ghost mode.

> *\*NOTE: Not all monsters will have a primary and secondary. Some monsters attack by just being near the player.*


![jester](https://i.imgur.com/a5VPz36.gif)

## Monster abilities
| Monster      | Primary | Secondary | Unique
| ----------- | ----------- | ----------- | -----------
| Baboon Hawk      | N/A       | Pickup/drop items | N/A
| Bracken | Drop body (if any) | N/A | N/A
| Coil-Head | N/A | (HOLD) Force move | N/A
| Company Monster | Tentacle attack | N/A | N/A
| Earth Leviathan | N/A | Emerge | N/A
| Eyeless Dog | N/A | N/A | N/A
| Forest Keeper   | N/A        | N/A | N/A
| Hoarding Bug   | Use held item        | Pickup/drop items | N/A
| Hygrodere   | N/A        | N/A | N/A
| Jester   | N/A        | (HOLD) Wind the music box | N/A
| Masked | N/A | N/A | Enter/leave facility (*'use' key*)
| Nutcracker   | Fire shotgun        | (HOLD) Sentry mode | N/A
| Snare Flea   | Drop (while on ceiling)        | Attach to ceiling | N/A
| Spore Lizard   | Stomp        | Smoke | N/A
| Thumper   | N/A        | Make noise | N/A

## Extended mode
To enable the Extended mode, **press ('0' digit key)** while in Player mode. This mode provides a few more options while in Player mode and will also enable the [experimental monsters](#experimental-monsters).

- Enables ALL monsters.
- **'8'**: Give +1000 credits.
- **'9'**: Teleport inside the main entrance.

## General config

| Option | Description |
| ----------- | ----------- |
| `use_enemy_spawning_behaviour` | If `true`, will spawn indoor enemies at a random vent and outdoor enemies at a random outdoor node (default `false`)
| `disable_mod_for_self` | If `true`, will disable the mod if you are hosting (default `false`)
| `force_push_to_talk_in_monster_mode` | If `true`, will force mic to be push-to-talk while in monster mode (default `true`)

## Keybind configuration
If you want to rebind the keybindings you can do so by modifying the `BepInEx/config/ControlCompany.ControlCompany.cfg` file. If you don't see this file then you must start the game to generate this file.

If you would like to revert the changes to the default settings, just delete the file and restart the game.


| Key      | Config key value example | 
| ----------- | ----------- |
| letters      | a      
| numbers   | 0
| num pad numbers   | num 0   
| function keys | f1
| arrow keys | up/left/down/right
| ctrl | ctrl (or right ctrl)
| alt   | alt (or right alt)  
| shift   | shift (or right shift)  
| space   | space      
| esc   | esc   
| caps lock   | caps lock        
| num lock   | num lock      


## Installation
1. Install [BepInEx](https://thunderstore.io/package/bbepis/BepInExPack/). This is used to load and run the mod.
2. Download this mod and place the `ControlCompany.dll` into your `BepInEx/plugins` folder.

## FAQ
### I want to filter out ControlCompany-enabled lobbies from my server list
By default if you have the mod installed then all servers of other players using ControlCompany will be highlighted in your server list. If you (as the host) do not want to use the mod you can disable the mod using the `disable_mod_for_self` config option.

### I installed the mod, why is the mod UI is not showing up?
Two possible reasons.
1. Host the lobby and pull the lever to start the mod. You should see the UI if you are hosting.
2. You toggled the UI off, press the UI toggle key to show the UI again (*default 'u'*)

### Does the mod work in multiplayer lobbies?
Yes.

### Does everyone need to have the mod?
**No! Absolutely not.** Only the game host (i.e. you) needs to run the mod! Where's the fun if everyone knows you're controlling the monster? ;)

### Do I need to host the game for the mod to work?
Yes, to give you the ability to spawn and control the monsters you **must host the lobby**. If you are not the host of a lobby the mod will show you an error message.

### Why can't I see a certain monster while in Ghost mode?
There are three possible cases. 
1. The monster is not available in the mod (yet).
2. The current map does not allow that monster to be spawned. For example, you cannot spawn the Jester in Vow because it cannot normally spawn in Vow.
3. The monster is an indoor/outdoor monster and the Ghost mode is not indoor/outdoor respectively. For example, you cannot spawn a Nutcracker outside.

### Can I control monsters while my real body is dead?
Yes, in fact it would be easier to play while dead so you won't have to worry about your body just standing there. You can talk to and hear other dead players while in ghost/monster mode.

### How do I rebind my keys?
See section on [Keybind configuration](#keybind-configuration).

### Will you add more monsters in the future?
Yes! We will add monsters and update the mod as we work out some of the issues. The current list are all the monsters we feel are stable. 


> *\*NOTE: If you would like to access ALL monsters in the game you can do so by enabling [Extended mode](#extended-mode). Going back into Ghost mode will show the list of ALL monsters in the game for the current map.*

## Report bugs/issues/requests

Please report any bugs and issues you encountered while using the mod or make a request by creating an issue on the [official GitHub repo issues page](https://github.com/ControlCompany/ControlCompany/issues). Thank you! :)

## Special thanks

A special thanks goes to the following people for their contributions to the development of the mod:

- **Quincy**: For thoroughly testing every corner of the mod since release day! Your contributions have definitely helped improve the mod!

## Changelog

### v1.1.9
- Added ***Obunga*** to the experimental list. Yes he's in the game files
- Moved the Eyeless Dog to the stable list
- Controlled monsters will now smoothly turn when moving, in addition you can look around without turning the monster
- Using the terminal will now disable control hotkeys
- **Rework**: The controlled Jester will now slowly ramp up its move speed while hunting

### v1.1.8
- Update mod version string

### v1.1.7
- Added a config option `use_enemy_spawning_behaviour` where if set to `true` (default `false`) will spawn the monsters at a random vent (if inside) or a random outdoor node (if outside)
- Camera in ghost/monster modes will now respect graphic settings of the player camera. For example, using HDLethalCompany will now also affect the ghost/monster cameras
- Servers created with the mod will now have the "[MODDED]" prefix
- Instead of hiding ControlCompany-enabled servers, it will now highlight the server that has it enabled
- Fixed an issue where loading monsters in modded maps may prevent the monster list from refreshing

### v1.1.6
- Added the Company Monster to the stable list. Yes you can control the Company Monster now
- Fixed issues where jumping over objects/railings can sometimes cause de-syncing issues
- **Dont Touch Me mod compatibility**: You can now spawn as the box

### v1.1.5
- If you have the mod installed then other ControlCompany-enabled servers will now be filtered out from **your view** of the public server list by default 
- Forcing push-to-talk while in ghost mode / monster mode can now be toggled off in the config
- Ghost and monster modes now use the in-game bindings for movement and sprinting
- **LC Office mod compatibility**: Fixed an issue where having the LC Office mod will cause the extended mode to break, yes you can now be a "shrimp".. kinda

### v1.1.4
- Added the Earth Leviathan to the stable list! Use the secondary skill to emerge! This is a single-use ability
- Fixed an issue where the Masked would naturally appear on moons that shouldn't have been possible
- Slightly increased the walk and run speed of the Forest Keeper

### v1.1.3
- Coil-Head has been moved to the stable list! You won't be able to move while anyone is looking at you unless you hold the secondary skill which forces the movement
- Opimized rendering while in ghost and monster modes, game should run much smoother while in those modes
- Added ability for the Masked monster to crouch (*in-game crouch key*), you cannot move while crouched. This is a limitation due to the game's lack of crouch movement animiation for the Masked monster
- Changed keybinds for the Masked monster to match the keybinds for the player
- Changed so you cannot move while you're in the kill animation for the Masked and Bracken

### v1.1.2
- Reverting change on only working in private lobbies. While griefing lobbies is an issue I would like to address, I will need to think of a better approach to this issue

### v1.1.1
- ~~The mod now only works if you are **hosting a PRIVATE lobby**, this is an intentional change done to prevent griefing public lobbies~~ (*reverted in v1.1.2*)
- The Masked enemy has been moved to the stable list! You'll be able to enter/leave the facility by pressing the "Use key" (*default 'E'*) on the door or colliding with the door
- Extended mode will now enable ALL monsters across ALL maps, however monsters are still bounded by whether they are considered an indoor/outdoor monster. For example, you can play the Jester in Experimental, but you cannot play the Jester outside
- Monsters can now jump
- Monsters can no longer walk through doors, instead they will automatically open doors on collision
- The 'Give credits' extended function will now increase the credits by 1000 each time it's pressed (as opposed to setting it to 5000)
- Fixed an issue with flipping extended mode on/off would not refresh the monster list

### v1.1.0
- Fixed issue where using ghost mode at the company building would prevent the UI from showing

### v1.0.9
- Fixed an issue where entering and leaving the facility and then using ghost mode may cause a soft lock if there are more than 12 spawnable monsters on the map
- Fixed an issue where you can still move the camera if the monster you are controlling dies

### v1.0.8
- Added Nutcracker reloading, he will now reload after emptying his shotgun
- Added the ability for the Baboon Hawk to pick up items as their secondary skill (*default 'RMB'*)
- Fixed an issue where the audio would be muffled while in ghost and monster mode
- Fixed an issue where if there were more than 12 monsters then some monsters would be unavailable. You can now scroll through the entire list of monsters using the left and right cycle keys (*default 'O' and 'P' respectively*) This was only an issue when there were modded monsters
- Fixed an issue where the Hoarding Bug would not attack the player if the bug was in aggro mode
- Fixed an issue where the Snare Flea would not attach to the player after dropping from the ceiling
- Fixed an issue where using the "Teleport to entrance" extended function would not remove weather effects while indoors
- The keybind config should now generate when the game launches, in addition any keybind changes will be reloaded when you create a new lobby

### v1.0.7
- Fixed an issue where you could potentially get stuck as ghost mode in the ship before it lands
- Fixed an issue where you could spawn outdoor enemies indoors and vice-versa if the current target enters/leaves the facility

### v1.0.6
- Everyone's favourite neck-snapping monster is out! The Bracken has been moved to the stable list!
- You can no longer target and spawn the ghost on dead players
- Added the ability to hide the "not host" text when you're not hosting. The text also disappears by itself after 30 seconds
- Fixed issue where the Thumper would bite players in different rooms
- Fixed most de-syncing issues affecting a few monsters

### v1.0.5
- Fixed some issues with different keyboard layouts causing crashes
- Rolled back changes to Hoarding Bug in v1.0.4 that was causing item sync issues. Investigating issue

### v1.0.4
- Added keybind configuration
- Added a toggle UI button *(default 'u')*
- Added a "lock enemy rotation" button *(hold left alt)*
- Improved Hoarding Bug pickup consistency and increasing pickup radius
- Fixed issue with accidentally voting to leave early when holding down RMB while in monster mode

### v1.0.3
- Hoarding bug will now be able to pickup/drop items as well as use items held

### v1.0.2
- Adjusted gravity of ghost and monsters

### v1.0.1
- Prevented Forest Keeper from moving when eating

### v1.0.0
- Initial release

