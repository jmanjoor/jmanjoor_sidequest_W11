## Project Title

## GBDA302 Week 11 Side Quest: Reflective Blob Platformer Testing Tools

## Authors

Starter code provided by Dr. Karen Cochrane and David Han
Modified and extended by Jowan Manjooran Jomon

---

## Description

This project builds on the Week 6 blob platformer and extends it with additional testing and debugging tools.

The player controls a small character navigating a side-scrolling world with collectibles, enemies, and hazards. The game includes:

Debug HUD: A toggleable overlay that displays live game information such as player position, velocity, health, score, active enemies, collectibles, and recent event logs. Hitboxes for the player, enemies, and collectibles can also be visualized to support collision testing.

Restart Key: Pressing R instantly resets the level and all player state at any point during play, allowing fast iteration without navigating a menu.

Slow Motion Mode: Pressing M toggles between normal speed (60 fps) and slow motion (15 fps), making it easier to observe jump arcs, collision timing, and enemy behaviour frame by frame. A badge appears in the debug HUD when active.

Stat Tracker: The debug HUD includes a live STATS panel showing deaths, total hits taken, and time survived this session. These update in real time as you play.

Playtest Logging: Pressing L dumps a formatted snapshot of all session stats (deaths, hits taken, time survived) to the browser console for easy review after a test run.

Audio Integration: Background music and sound effects are connected to gameplay events such as jumping, collecting items, and taking damage.

Modular Architecture: The game uses a modular structure where systems such as input, camera, sound, and gameplay logic are separated. JSON configuration files control level setup and behavior, allowing flexible changes without modifying core code.

## These additions improve testing, debugging, balancing, and overall clarity of the gameplay experience.

## Controls

Arrow Keys / WASD – Move  
Arrow Up – Jump  
Space – Attack  
D – Toggle Debug HUD  
I – Toggle invincibility  
M – Toggle slow motion  
R – Restart level  
L – Log playtest stats to console

## Learning Goals

- - Implement toggleable testing and debug tools to support development
- - Use a debug HUD to visualize game state and hitboxes
- - Add a slow-motion feature to better inspect gameplay interactions
- - Maintain modular game structure and system separation
- - Implement sprite sheet animations for characters and objects
- - Use tilesets for environment graphics
- - Add and connect sound effects and background music to gameplay events
- - Use event-driven programming to track game actions
- - Load and parse level data from JSON files
- - Structure a p5.js project with clear separation between world logic, rendering, and system modules

## Assets

The following external assets were used:

Sprite Sheets

- - Player character sprite sheet (Blob) - https://craftpix.net/freebies/free-slime-sprite-sheets-pixel-art/
- - Enemy sprite sheet (Slime Mobs) - https://craftpix.net/freebies/free-slime-sprite-sheets-pixel-art/
- - Leaf collectible sprite sheet - https://craftpix.net/freebies/free-slime-mobs-pixel-art-top-down-sprite-pack/

Tileset - https://craftpix.net/freebies/free-green-zone-tileset-pixel-art/

- - Ground tiles
- - Platform tiles
- - Wall tiles

Sound Effects

- - Jump sound https://mixkit.co/free-sound-effects/discover/attack/
- - Attack sound - https://mixkit.co/free-sound-effects/discover/attack/
- - Item collection sound https://mixkit.co/free-sound-effects/discover/attack/
- - Damage sound https://mixkit.co/free-sound-effects/discover/attack/

Background music  
Background music used for gameplay atmosphere already provided

All assets used are free or educational-use assets and are credited to their original creators.

## GenAI

Starter code was provided by Dr. Karen Cochrane and David Han.

- - Generative AI tools were used to support the development process by:
- - helping understand the structure of the provided starter code
- - assisting with debugging sprite loading and animation configuration
- - explaining how JSON configuration files interact with the game systems
- - helping integrate sound effects through the event-driven architecture
- - clarifying how different modules in the project communicate with each other
- - helping implement and troubleshoot slow motion as a testing feature
- - helping extend the debug system for easier gameplay testing

Claude was used to support implementation and debugging for the added testing tools.

All final implementation decisions and integration were completed by the author.
