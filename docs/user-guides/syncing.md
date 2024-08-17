---
sidebar_position: 2
---

# Sync Your Account

Account syncing allows for your [autoroles](/guild-guides/configure-autoroles), [linked role](/guild-guides/configure-guild-linking#configure-linked-role), and [nickname](/guild-guides/configure-guild-linking#toggle-nickname-syncing-on--off) to be updated (across guilds that have IsleStats configured) to reflect the profile of the player that you are linked to.

## How Syncing is Triggered

There is a few different ways syncing can be triggered:

- When you join a Discord guild that IsleStats is in.
- When the player linked to your Discord account is looked up.
- When you run the IsleStats `/sync` command.
- When you link to a player.

:::info
There is a 15 minute cooldown between syncing attempts.
:::

### Syncing via player lookup

Player lookup based syncing updates autoroles based on the API category looked up, see [Enable the MCCI Island API](/user-guides/enable-mcci-api) for more info.

When a player's MCC Island information is looked up via an IsleStats command (eg. `/currency`), syncing is triggered for category that was looked up. This means that if your linked player's currency info is checked, your autoroles for the collections category will update. This is because a player's currency info is part of the collections category.

Cooldowns operate on a per-category basis, this means that the syncing cooldown for the collection category is seperate from that of the statistics category.

Uncategorised information as well as your linked role and nickname will be updated regardless of the lookup.

:::note
The same is true for stats commands such as `/skybattle stats`. Because these commands look up information from the statistics group, autoroles for the statistics category will update.
:::

### Syncing via the `/sync` command

Running the IsleStats `/sync` command will trigger full sync for all autoroles, linked roles, and nicknames across all guilds with IsleStats configured.

There is a 15 minute cooldown on this command. This cooldown is shared with other syncing trigger methods, meaning that if a full sync is triggered by other means, you won't be able to use the `/sync` command for 15 minutes after.
