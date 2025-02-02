# QWERTZcore Documentation

## Overview

QWERTZ Core is an all-in-one event management plugin for Minecraft servers. It provides a comprehensive set of tools for hosts and administrators to manage events, player statuses, and game mechanics.

**Newest version:** 1.1
**Author:** QWERTZ_EXE
**Website:** https://qwertz.app

## Features

- Event countdown and timer management
- Player revival system with tokens
- Gamemode management
- Inventory management for alive/dead players
- Player visibility controls
- A lot of Configuration options
- Optional Luckperms features
- Placeholder API support
- Database for tracking wins and revive tokens

## Commands

### General Commands

- `/core` - Displays information about QWERTZ Core
- `/config <key> <value>` - Edit configuration values
- `/hide <host|staff|all|off>` - Hide other players based on their rank
- `/spawn` - Teleport to spawn location
- `/discord` - Displays the discord invite set in the config
- `/message <player> <message>` - Private messages a player
- `/reply <message>` - Reply to the last player who messaged you
- `/togglemessage` - Toggles incoming private messages
- `/mutechat` - Mute the chat
- `/unmutechat` - Unmute the chat
- `/ad <platform>` - Broadcast an advertisement
- `/wins [player]` - Check the wins of a player
- `/revives [player]` - Check the revive tokens of a player
- `/warp <warp>` - Warp to a warp
- `/warps` - List all available warps
- `/setwarp <warp>` - Create a warp
- `/delwarp <warp>` - Delete a warp
- `/setad <platform> <advertisement>` - Set an advertisement for a platform

### Event Management

- `/timer <seconds|cancel>` - Starts or cancels a countdown timer
- `/eventcountdown <time|cancel>` - Start or cancel a countdown for the event

### Gamemode Commands

- `/gmc` - Set gamemode to creative
- `/gms` - Set gamemode to survival
- `/gmsp` - Set gamemode to spectator
- `/gma` - Set gamemode to adventure
- `/gm <creative|survival|adventure|spectator>` - Set gamemode

### Revival System

- `/chatrevive <math|typer|guess> [max]` - Start a chat revival game
- `/revive <player>` - Revive a player
- `/unrevive <player>` - Mark a player as dead
- `/reviveall` - Revive all players
- `/revivelast [seconds]` - Revives all players who died in the last specified number of seconds
- `/userevive` - Request to use a revive token
- `/reviveaccept <player>` - Accept a player's revive request
- `/revivedeny <player>` - Deny a player's revive request
- `/addrevive <player>` - Add a revive token to a player
- `/removerevive <player>` - Remove a revive token from a player

### Player Management

- `/listalive` - List all alive players
- `/listdead` - List all dead players
- `/givedead <item> [amount] [data]` - Give an item to all dead players
- `/givealive <item> [amount] [data]` - Give an item to all alive players
- `/tpalive` - Teleport all alive players to you
- `/tpdead` - Teleport all dead players to you
- `/tphere <player>` - Teleport the selected player to you
- `/clearalive` - Clears the inventory of all alive players
- `/cleardead` - Clears the inventory of all dead players
- `/healalive` - Heals all alive players
- `/healdead` - Heals all dead players

### Database Management

- `/addwin <player>` - Add a win to a player's record
- `/removewin <player>` - Remove a win from a player's record

## Permissions

### Basic Permissions

- `qwertzcore.host.*` - All host permissions
- `qwertzcore.staff.*` - All staff permissions
- `qwertzcore.player.*` - All player permissions
- `qwertzcore.gamemode.*` - All gamemode permissions
- `qwertzcore.config.*` - All config permissions
- `qwertzcore.database.*` - All database permissions

### Specific Permissions

#### Host Permissions

- `qwertzcore.host.timer` - Manage timers
- `qwertzcore.host.revival` - Manage chat revivals
- `qwertzcore.host.revive` - Revive players
- `qwertzcore.host.unrevive` - Unrevive players
- `qwertzcore.host.reviveall` - Revive all players
- `qwertzcore.host.listalive` - List alive players
- `qwertzcore.host.listdead` - List dead players
- `qwertzcore.host.givedead` - Give items to dead players
- `qwertzcore.host.givealive` - Give items to alive players
- `qwertzcore.host.tpalive` - Teleport alive players
- `qwertzcore.host.tpdead` - Teleport dead players
- `qwertzcore.host.tphere` - Teleport a player
- `qwertzcore.host.clearalive` - Clear alive players' inventories
- `qwertzcore.host.cleardead` - Clear dead players' inventories
- `qwertzcore.host.healalive` - Heals alive players
- `qwertzcore.host.healdead` - Heals dead players
- `qwertzcore.host.revivelast` - Revive recently dead players
- `qwertzcore.host.eventcountdown` - Manage event countdowns
- `qwertzcore.host.reviveaccept` - Accept revive requests
- `qwertzcore.host.revivedeny` - Deny revive requests
- `qwertzcore.host.addrevive` - Add revive tokens
- `qwertzcore.host.removerevive` - Remove revive tokens
- `qwertzcore.host.mutechat` - Mute the chat
- `qwertzcore.host.unmutechat` - Unmute the chat
- `qwertzcore.host.ad` - Broadcast an advertisement

#### Player Permissions

- `qwertzcore.player.spawn` - Use spawn command
- `qwertzcore.player.hide` - Use hide command
- `qwertzcore.player.discord` - Use discord command
- `qwertzcore.player.userevive` - Use revive tokens
- `qwertzcore.player.checkrevives` - Check revives
- `qwertzcore.player.checkwins` - Check wins
- `qwertzcore.player.message` - Private message and reply to others
- `qwertzcore.player.togglemessage` - Toggle incoming private messages
- `qwertzcore.player.listwarps` - List all available warps
- `qwertzcore.player.warp` - Use warps

#### Gamemode Permissions

- `qwertzcore.gamemode.creative` - Use creative mode
- `qwertzcore.gamemode.survival` - Use survival mode
- `qwertzcore.gamemode.spectator` - Use spectator mode
- `qwertzcore.gamemode.adventure` - Use adventure mode
- `qwertzcore.gamemode` - Use general gamemode command

#### Config Permissions

- `qwertzcore.config` - Edit plugin configuration
- `qwertzcore.config.setad` - Set an advertisement
- `qwertzcore.config.setwarp` - Set a warp
- `qwertzcore.config.delwarp` - Delete a warp

#### Database Permissions

- `qwertzcore.database.addwin` - Add wins to players' records
- `qwertzcore.database.removewin` - Remove wins from players' records

#### Other Permissions

- `qwertzcore.chat.bypass` - Bypass a muted chat
- `qwertzcore.chat.bypasstm` - Bypass the disabled vanilla commands /tm and /teammsg
- `qwertzcore.chat.bypassme` - Bypass the disabled vanilla command /me

## Placeholders

- `%qwertzcore_alive%` - Amount of alive players
- `%qwertzcore_dead%` - Amount of dead players
- `%qwertzcore_isalive%` - "true" if the player is alive, else "false"
- `%qwertzcore_isdead%` - "true" if the player is dead, else "false"
- `%qwertzcore_revives%` - Amount of revives the player has
- `%qwertzcore_wins%` - Amount of wins the player has
- `%qwertzcore_server%` - Server name configured in the config
- `%qwertzcore_event%` - Current event
- `%qwertzcore_startingin%` - Formatted string displaying the time until the event starts

# Links
[Modrinth](https://modrinth.com/plugin/qwertz-core/) | [bStats](https://bstats.org/plugin/bukkit/QWERTZ%20Core/23512) | [GitHub](https://github.com/QWERTZexe/QWERTZ-Core)