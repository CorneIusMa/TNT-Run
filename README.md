Tested Major MC Versions:
1.81.91.101.111.121.131.141.151.161.171.181.191.201.20.61.21
Source Code:
https://github.com/CorneliusMa/SilkSpawners_v2
Languages Supported:
English, German, Turkish, Indonesian

[​IMG]
SilkSpawners​
If you use a pickaxe with the silk touch enchantment while breaking a spawner, you will receive the spawner you broke. When placing the spawner again, the spawner will spawn the mob it spawned when breaking it.

Commands
/silkspawners help [command]
/silkspawners give <Player> <Type> [Amount]
/silkspawners set <Type>
/silkspawners explosion <enable/disable/setting> <Player>
/silkspawners locale <setting/reload/update>
/silkspawners entities
/silkspawners version

Permissions
Commands

silkspawners.command.give - Use this command to give spawners to players.
In addition set silkspawners.command.give.* to allow all entites or replace the star with an entity name.​
silkspawners.command.set - Use this command to change already
placed spawners.
In addition set silkspawners.command.set.* to allow all entites or replace the star with an entity name.​
silkspawners.command.explosion - Use this command to temporarily enable or disable spawner explosions for a specific player.
silkspawners.command.locale - Use this command, to reload and update locale files.
silkspawners.command.entities- Use this command to see the entities you can use in permissions and commands.
silkspawners.command.version - Use this command to see, if updates are available.
Click to expand...
Spawners

silkspawners.break.* - Permission to set, if players will receive destroyed spawners.
silkspawners.place.* - Permission to set, if players can place silk spawners.
silkspawners.change.* - Permission to set, if players can change spawners with eggs.
silkspawners.explosion - If set, spawner explosion is enabled.
If you want to allow only specific types of spawners you can replace the * with an entity name. Use the entities command to see spawnable entites.


Configuration

Default configuration:
Code (YAML):
messages:
  prefix: $8[$bSilkSpawners$8] # The plugin prefix used in all messages
  locale: en # The locale file to be used
spawner:
  dropChance: 100 # Probability that the spawner will drop when mined (0-100)
  destroyable: true  # If set to false, it won't be possibile to destroy spawners without SilkTouch or whitout the permission
  pickaxeRequired: true # If set to false, spawners will always drop regardless of what the player is holding in his hand
  silktouchRequired: true # If set to false, spawners will drop even if the used pickaxe does not have SilkTouch
  item:
    name: $dSpawner # The name of the spawner item dropped
    prefix: $e # The text before the spawner name in the lore
    prefixOld: '' # If you change your prefix, set this value to your old prefix  to keep existing spawners functional
    lore: [] # Set an array for this value to set a custom lore
  explosion:
    normal: 0 # The explosion intensity when spawners are mined without SilkTouch
    silktouch: 0 # The explosion intensity when spawners are mined with SilkTouch
  message:
    denyDestroy: true # If set to true, a message will be sent to the player if the spawner cannot be destroyed
    denyPlace: true # If set to true, a message will be sent to the player if the spawner cannot be placed
    denyChange: true # If set to true, a message will be sent to the player if the spawner cannot be changed
  permission:
    disableDestroy: false # If set to true, no permission is required to receive destroyed spawners
    disablePlace: false # If set to true, no permission is required to place spawners
    disableChange: false # If set to true, no permission is required to change spawners with eggs
update:
  configVersion: 2 # Do not change this value manually! It is automatically managed by the plugin
  check:
    enabled: true # If set to true, the plugin will check for updates
    interval: 24 # The interval in hours at which to check for updates
If you want to use a dollar sign in a value, you can do so by putting a backslash in front of it.
Click to expand...


Custom messages
To protect your locale files from unwanted overwriting, you must manually update the locale files with the /silkspawners locale command after an update.

If you want to create your own locale file, you should create a new file to prevent your changes from being overwritten when you update the locale files.
Locale files must be named accordingly to the messages_myfile.properties naming schema and can be used setting myfile as locale.

Spoiler: Default messages file
[​IMG]
If you have created your own translation, it would be awesome if you could submit it at our translation program, so other people can use it too.

Tutorial


Thanks to KasaiSora for creating this great tutorial!


Spoiler: Statistics (since May 17, 2022)

This plugin also supports Folia.
brius_xD, Jsaunders411, rektas and 6 others like this.
Recent Updates
Version 2.3.2 Dec 11, 2024
Version 2.3.1 Aug 10, 2024
Version 2.3.0 Aug 6, 2024
