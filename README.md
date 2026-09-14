<h1>
    <img src="worldguard-logo.svg" alt="WorldGuard" width="400" /> 
</h1>

A fork of [WorldGuard](https://github.com/EngineHub/WorldGuard) 7.0.8 maintained by [TrueOG Network](https://true-og.net) for 1.19.4. WorldGuard lets you and players guard areas of land against griefers and undesirables, as well as tweak and disable various gameplay features of Minecraft.

## Changes over WorldGuard:

- Gradle 8.0.2 -> 8.14.3.
- `build` copies the shaded jar to `build/libs/WorldGuard-<version>.jar` via `copyjar.sh`.
- Ships the live TrueOG Network `config.yml`, `config_world.yml`, and `worlds/world/regions.yml` as defaults. The world regions file is created on first run alongside the main config.
- New region flag `creeper-block-damage` (default allow). Set it to deny with `creeper-explosion` allowed to keep creeper blasts from breaking blocks while still damaging entities. This is how the spawn warzone is configured.
- Bucket use no longer plays the deny effect when a partner plugin's `safe-fluids` flag allows the action (FireFight-OG compatibility).

## Upstream description:

* Block creeper and wither block damage, falling damage, etc.
* Disable fire spread, lava fire spread, ice formation, Endermen picking up blocks, etc.
* Blacklist certain items and blocks so they can't be used
* Warn moderators when certain items and blocks are used
* Protect areas of your world so only certain people can build in them
* Set areas where PVP, TNT, mob damage, and other features are disabled
* Protect your server from various 'exploits' like magical obsidian creation machines
* Disable, or enable, various Minecraft features, like sponges from classic
* Add useful commands like an immediate "STOP ALL FIRE SPREAD" command
* Enable only features you want! Everything is off by default

WorldGuard is open source and is available under the GNU Lesser
General Public License v3.

A Bukkit server implementation (such as [Paper](https://papermc.io)) and the [WorldEdit plugin](https://dev.bukkit.org/projects/worldedit) are required to use WorldGuard. You can get a release copy of WorldGuard from the [BukkitDev site](https://dev.bukkit.org/projects/worldguard).

Compiling
---------

The project is written for Java 17 and our build process makes use of
[Gradle](http://gradle.org). Run `./gradlew build` and pick up the plugin jar from `build/libs/`.

Dependencies are automatically handled by Gradle.

Contributing
------------

We happily accept contributions, especially through pull requests on GitHub.

Please read CONTRIBUTING.md for important guidelines to follow.

Submissions must be licensed under the GNU Lesser General Public License v3.

Links
-----

* [TrueOG fork](https://github.com/true-og/WorldGuard)
* [Homepage](http://enginehub.org/worldguard)
* [Discord](https://discord.gg/enginehub)
* [Issue tracker](https://github.com/EngineHub/WorldGuard/issues)
* [Continuous integration](http://builds.enginehub.org) [![Build Status](https://ci.enginehub.org/app/rest/builds/buildType:bt11,branch:master/statusIcon.svg)](http://ci.enginehub.org/viewType.html?buildTypeId=bt11&guest=1)
* [End-user documentation](https://worldguard.enginehub.org/en/latest/)
