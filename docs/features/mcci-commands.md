---
sidebar_position: 1
description: Commands that allow you to view MCCI player information.
---

# MCCI Commands

## Statistics Commands

IsleStats offers a range of commands for different MCCI gamemodes. These commands include statistics and badges for each gamemode.

Supported gamemodes are:

- Sky Battle (`/skybattle`)
- Battle Box (`/battlebox`)
- Dynaball (`/dynaball`)
- Parkour Warrior (`/parkourwarrior`)
- Hole in the Wall (`/holeinthewall`)
- Rocket Spleef Rush (`/rocketspleefrush`)
- To Get to the Other Side (`/tgttos`)

Each of these command groups have two sub commands:

- `stats` - this allows you to view gamemode statistics like wins and kills.
- `badges` - this allows you to view badges obtained in the gamemode.

### Parameters

- `player` - the player to view the stats / badges of.

:::note
These commands require API visibility for **statistics** to be enabled. See [Enable the MCC Island API](/user-guides/enable-mcci-api) for more info.
:::

## Currency Info

**Usage**: `/currency [<player>]`

The `/currency` command displays information on a player's MCCI currencies. It includes:

- Coins
- Silver
- Material dust
- Royal reputation
- Gems

### Parameters

- `player` - the player to currency info of.

:::note
These commands require API visibility for **collections** to be enabled. See [Enable the MCC Island API](/user-guides/enable-mcci-api) for more info.
:::

## Leveling Info

**Usage**: `/leveling [<player>]`

The `/leveling` command shows the amount of trophies obtained by a player in each category, as well as a level progress bar.

### Parameters

- `player` - the player to leveling info of.
