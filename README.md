# Kadlecova-G300-Midterm

**Project Name:** Kadlec_Midterm  
**Theme:** *Sacrifices Must Be Made*

## Overview

This gameplay prototype was developed for the G300 midterm assignment, centered on the theme "Sacrifices Must Be Made." The player explores a haunted graveyard, tasked with destroying all pumpkins to escape. Along the way, they must avoid enemies, manage limited resources, and answer a final question from a witch NPC that determines their fate.

Assets from the PolyPerfect Halloween Free Pack were used to provide consistent and stylized Halloween visuals, including characters, props, and environmental elements.

## Core Gameplay

The player moves through a graveyard and must destroy all pumpkins using three types of throwable projectiles. At the end of the level, they encounter a witch NPC who automatically initiates a dialog. The witch asks if the player has destroyed all pumpkins. Based on the player’s response:
- If correct → the Win screen is shown
- If incorrect → the Game Over screen is triggered

Meanwhile, the player must:
- Switch between projectiles (1, 2, 3)
- Aim by holding E and throw by releasing E
- Avoid a ghost enemy that patrols waypoints and chases the player if detected
- Collect mushrooms to restore lost health
- Manage limited ammunition and collect ammo pickups

The game features:
- A Main Menu with listed controls
- A playable Main Level
- Game Over and Win screens, triggered by gameplay outcome

## Implemented Features

### Theme Cohesion (2 Points)
The concept of sacrifice is directly implemented in the game loop. The pumpkins—presented as friendly companions—must be destroyed to complete the game. The visual tone, particle effects, sounds, and final NPC interaction reinforce this theme throughout.

### Coherent Level Design (1 Point)
The level uses clear visual guidance and spatial layout to direct the player. There are no mazes. The witch NPC at the end is positioned as a final checkpoint both visually and narratively.

### Collectibles and Score UI (1 Point)
Destroying a pumpkin increases the player's score. The current score is displayed via a UI widget throughout the game.

### AI Patrol and Chase System (2 Points)
A ghost enemy follows preset waypoints. If it detects the player, it switches to chase mode. On contact, the ghost damages the player by reducing health.

### Timelines (1 Point)
A Timeline is used to animate mushrooms, creating a pulsing visual effect to attract player attention and indicate they can be collected for healing.

### Menus and Scene Management (1 Point)
- A Main Menu lists controls before entering gameplay
- The game ends in either a Win or Game Over screen, depending on the player’s answer to the NPC question

### NPC Dialogue and Interaction (2 Points)
At the end of the level, the player automatically triggers a dialog sequence with the witch NPC by entering her area. The witch asks a question based on gameplay: "Have you destroyed all pumpkins?" A correct answer ends the game successfully. A wrong answer results in the player's death and Game Over.

### Projectile and Health System (2 Points)
The player uses throwable projectiles, aimed manually by holding E and thrown on release. Targets like pumpkins use a health component and require multiple hits. Enemy/object health is displayed via a health bar.

### Ammo System (2 Points)
- The player starts with limited ammo
- Ammo pickups are placed in the environment
- Current ammo is displayed on screen
- Shooting is disabled when ammo reaches zero

### Player Health and Death System (2 Points)
The player has a visible health bar. Health is lost when:
- The ghost enemy catches the player

Health can be restored by collecting mushrooms placed in the level. If health reaches zero, the game transitions to the Game Over screen.

## Additional Features (4 Points)

### 1. Multiple Weapon Types (2 Points)
The player can press 1, 2, or 3 to switch between three different projectile types, each offering distinct visuals or behavior.

### 2. Exit Unlock Based on Objective (2 Points)
The player can access the final NPC at any time, but if they have not destroyed all pumpkins, their answer to the witch’s question will be incorrect, resulting in a Game Over. This mechanic reinforces the core objective without blocking physical progression and ties gameplay resolution directly to the theme of sacrifice.

## Controls

- Move – W, A, S, D
- Aim – Hold E
- Throw Projectile – Release E
- Switch Projectiles – 1, 2, 3
- NPC Interaction – Automatic on proximity

