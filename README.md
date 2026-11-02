# CherryEssentials (BerryEssentials)

- Plugin name: `BerryEssentials`
- Output JAR name: `CherryEssentials.jar`
- Author: Berry
- Target: Paper 26.3 / Java 25
- API dependency: `io.papermc.paper:paper-api:26.3.build.+`
- No land-claim feature is included.

## Build

Install a JDK 25 and Gradle 8.14+ (or a compatible newer Gradle), then run from this directory:

```bash
gradle clean build
```

The output will be `build/libs/CherryEssentials.jar`. Put it in the server's `plugins/` directory and restart Paper.

## Implemented in this initial source build

- Custom purple/yellow BerryEssentials sidebar scoreboard
- Profile/server lines: name, money, clan, rank, online, TPS, K/D, dimension
- Persistent player wallet and bank balances
- `/money`, `/pay`, `/bank deposit|withdraw`
- `/sethome`, `/home`, `/delhome` with configurable default home limit
- Admin `/setwarp`, `/warp`, `/delwarp`
- `/tpa`, `/tpaccept` with expiry
- `/rtp` with configurable radius and safe-ground attempts
- Config-driven shop GUI with economy purchases
- Member menu GUI
- Persistent personal backpack
- Basic clan creation and leave
- Basic rank assignment command
- Basic kill quest counter / quest status

## Not implemented yet (do not advertise as working)

These requested systems need a further implementation/integration pass before this can be called feature-complete:

- Chest Shop (player-owned sign shops, stock, protection and transaction handling)
- Minimap support (specific provider/protocol integration; e.g. Dynmap/BlueMap/Pl3xMap markers)
- Custom NPC dialog (requires choosing an NPC provider such as Citizens, or a native interaction design)
- Full ranks & nametag color synchronization (including permission-plugin/Vault/LuckPerms integration)
- Full Battlepass with seasons, XP progression, rewards and persistence
- Full quest engine (configurable objectives, tracking, rewards, reset schedules)
- Full clan system (invites, members, roles, homes, chat, disband and permissions)
- Economy/shop administration, sell GUI, transaction logs, offline transfers and robust database migration
- Full admin/member menus and GUI configuration

This is an honest first implementation, not a claim that every requested feature is complete. Test on a disposable Paper 26.3 server and back up worlds/data before production use.
