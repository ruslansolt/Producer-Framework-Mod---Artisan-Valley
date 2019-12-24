![Producer Framework Migration Guide for Artisan Valley](https://i.imgur.com/cvDTlUD.png)

## Contents
* [Introduction](#introduction)
  * [What's New](#whats-new)
* [Installing Producer Framework Mod](#installing-producer-framework-mod)
* [Installing Artisan Valley 3.0](#installing-artisan-valley)
* [Manually Uninstalling Custom Farming Redux](#manually-uninstalling-custom-farming-redux)
  * [Artisan Valley is my only Custom Farming Redux mod](#artisan-valley-only)
  * [I have other Custom Farming Redux mods installed](#other-CFR-mods)
* [Questions](#questions)
  * [Can I keep using the CFR version of Artisan Valley?](#can-i-keep-using-the-cfr-version-of-artisan-valley)
  * [Do I really need to remove my CFR machines prior to uninstalling CFR?](#do-i-really-need-to-remove-my-cfr-machines-prior-to-uninstalling-cfr)
* [Documentation for Modders](#documentation-for-modders)
  * [How to use an Artisan Valley machine](#how-to-use-an-artisan-valley-machine)
  * [Migrating your CFR pack](#migrating-your-cfr-pack)

## Introduction

Since its inception, [Artisan Valley](https://www.nexusmods.com/stardewvalley/mods/1926) has used [Custom Farming Redux](https://www.nexusmods.com/stardewvalley/mods/991) as its second core framework. CFR gave us the ability to add custom machines into Stardew Valley but not modify vanilla machines. This lead to Artisan Valley having machines such as: Exotic Mayonnaise Machine, Hardwood Keg, and Vinegar Cask to name a few. It had always been the intention of being able to utilize the vanilla machines in tandem with non-vanilla inputs and outputs. [Producer Framework Mod](https://www.nexusmods.com/stardewvalley/mods/4970) gave us this opportunity while also being a more stable framework and built around the needs of the PPJA team. Digus has previously provided us with content packs for [Mail Framework Mod](https://www.nexusmods.com/stardewvalley/mods/1536) and the ability to age custom items in the vanilla casks with [Custom Cask Mod](https://www.nexusmods.com/stardewvalley/mods/2642). 

This guide also applies to [Farmer to Florist](https://www.nexusmods.com/stardewvalley/mods/2075) but I will refer to Artisan Valley primarily.

### What's New

Artisan Valley 3.0 adds some new features to hopefully extend the length of gameplay:

* Machines unlock based on certain skill levels
* Vanilla machines can now accept custom items
* Ability to age certain custom products in casks now (alcohol for example)

## Installing Producer Framework Mod

1. [Install the latest version of SMAPI](https://smapi.io/).
2. Install [Producer Framework Mod](https://www.nexusmods.com/stardewvalley/mods/4970).
3. Run the game using SMAPI.

## Installing Artisan Valley

This assumes you have installed Producer Framework Mod already.

1. Delete all pre-existing Artisan Valley folders ([CFR] Artisan Valley and [JA] Artisan Valley Machine Goods, inside [PPJA] Artisan Valley). This is important for [the tool](https://www.nexusmods.com/stardewvalley/mods/4972) to run properly.
2. [Install the latest version of Artisan Valley](https://www.nexusmods.com/stardewvalley/mods/1926) *Version 3.0 or later supports Producer Framework Mod.* Artisan Valley 3.0 has a mod that will automatically convert any pre-existing CFR machines into BigCraftables. If you're having trouble follow the [Manually Uninstalling CFR Guide](#manually-uninstalling-custom-farming-redux).
3. Install the latest version of: [Json Assets](https://www.nexusmods.com/stardewvalley/mods/1720), [SpaceCore](https://www.nexusmods.com/stardewvalley/mods/1348), [Mail Framework Mod](https://www.nexusmods.com/stardewvalley/mods/1536), [Content Patcher](https://www.nexusmods.com/stardewvalley/mods/1915), & [PPJA Collection](https://www.nexusmods.com/stardewvalley/mods/1935).
4. *Optional* Install [Custom Cask Mod](https://www.nexusmods.com/stardewvalley/mods/2642) to age alcohols in casks.
5. Unzip any folders and drop them into `Mods`
6. Run the game using SMAPI

__________________________

## Manually Uninstalling Custom Farming Redux

Artisan Valley & Farmer to Florist [has a tool](https://www.nexusmods.com/stardewvalley/mods/4972) that will automatically convert any pre-existing Artisan Valley or Farmer to Florist machines into BigCraftables or their vanilla counterpart. If you're having trouble with this mod below are two guide for manually uninstalling CFR.

Follow the guide depending on which situation applies to you. If the **only** Custom Farming Redux mod you have installed is Artisan Valley you will follow `Artisan Valley Only`. If you have other mods that use Custom Farming Redux you will follow `Other CFR Mods`.

Improper uninstallation will cause your machines to [turn into chests](https://i.imgur.com/DmoG3L6.png). You will not only lose the machine but the item inside. To learn more as to why you should follow the steps below see [here](https://github.com/paradigmnomad/Producer-Framework-Mod---Artisan-Valley#do-i-really-need-to-remove-my-cfr-machines-prior-to-uninstalling-cfr).

### Artisan Valley Only

If you're reading this, the only Custom Farming Redux mod you have installed is Artisan Valley.

1. [Backup your save file](https://stardewvalleywiki.com/Saves#Find_your_save_files). 
2. If you have any machines currently processing let them finish or break them with a tool to retrieve the item & machine. You can place the item that was inside in a chest as they will not be effected.
3. If you have any machines placed on your farm pick them up. 
4. If you have any machines in your chests remove them from chests.

⚠ At this point you should have all of your custom machines in your inventory ⚠

5. **DELETE ALL MACHINES** You can throw them in the trash, the river, down in the mines. You will need to sleep/save the game. If you don't want to have to re-craft everything make a note of what machines you have. You can spawn them in with [CJB Item Spawner](https://www.nexusmods.com/stardewvalley/mods/93) to save you from having to gather more resources.
6. Close the game and navigate to your `Mods` folder.
7. Remove the following two folders: `Custom Farming Redux` (should be directly in your `Mods` folder) and `[CFR] Artisan Valley` (may be located under `[PPJA] Artisan Valley`). 

### Other CFR Mods

If you're reading this you have other mods that use CFR. This means you **cannot** fully uninstall CFR.

1. [Backup your save file](https://stardewvalleywiki.com/Saves#Find_your_save_files). 

--- You will be removing only Artisan Valley machines. If you need a refresher of which machines Artisan Valley adds, check out [Mousey's PPJA and Friends Reference](https://mouseypounds.github.io/ppja-ref/machines.html) ---

2. If you have any Artisan Valley machines currently processing let them finish or break them with a tool to retrieve the item & machine. You can place the item that was inside in a chest as they will not be effected.
3. If you have any Artisan Valley machines placed on your farm pick them up. 
4. If you have any Artisan Valley machines in your chests remove them from chests.

⚠ At this point you should have all of your Artisan Valley machines in your inventory ⚠

5. **DELETE ALL ARTISAN VALLEY MACHINES** You can throw them in the trash, the river, down in the mines. You will need to sleep/save the game. If you don't want to have to re-craft everything make a note of what Artisan Valley machines you have. You can spawn them in with [CJB Item Spawner](https://www.nexusmods.com/stardewvalley/mods/93) to save you from having to gather more resources.
6. Close the game and navigate to your `Mods` folder.
7. Remove the following folder: `[CFR] Artisan Valley` (may be located under `[PPJA] Artisan Valley`). 

__________________________

## Questions

### Can I keep using the CFR version of Artisan Valley?
The last version of Artisan Valley to support CFR was 2.09. 3.0 fully migrates to Producer Framework Mod. You are welcome to continue to use this version however no further updates or support will be provided for the CFR version of Artisan Valley. 

### Do I really need to remove my CFR machines prior to uninstalling CFR?
Because of how CFR is written **YES**. If the pack a machine came from OR Custom Farming Redux itself is removed, the machine will turn into a chest to prevent the game from crashing because of a missing item. If you have an item processing, chances are you will have one or two items in that chest - the finished product if it is a non-prefixed or suffixed item such as Butter, or if it is a prefixed/suffixed item, you'll have the generic version of that item (`Essential Oil` for example) and the item that was going to give its unique identifier (`Herbal Lavender` for example). In short, it is up to you whether or not you rip your machines up before uninstalling, but there will be no ill effects if you do not.

__________________________

## Documentation for Modders

With the release of PFM you can now target machines outside of the pack, something CFR could not do. This means you do not have to have the PPJA team add your items to Artisan Valley's code to make it work. We have migrated some pre-existing packs over to this format:

* [Cannabis Kit](https://www.nexusmods.com/stardewvalley/mods/1741)
* [Sweet Tooth](https://www.nexusmods.com/stardewvalley/mods/1897)
* [BFAV Phoenixes](https://www.nexusmods.com/stardewvalley/mods/4846)
* [Trent's New Animals](https://www.nexusmods.com/stardewvalley/mods/3634)
* [Ancient Crop](https://www.nexusmods.com/stardewvalley/mods/4472)
* [Murrthecat's BFAV Quails](https://www.nexusmods.com/stardewvalley/mods/4847)

You will have to download these add-on packs seperate. 

### How to use an Artisan Valley machine
`"ProducerName"` has to match a unique name. If you want to use Artisan Valley Alembic you would type: `"ProducerName": "Alembic"`. You may also want to list Artisan Valley as a dependency in your manifest to ensure users have both installed. But that's it! You can now use any Artisan Valley machine.

You can also use any `ProducerName` from other mods (like [Farmer to Florist](https://www.nexusmods.com/stardewvalley/mods/2075) well.

### Migrating your CFR pack
If you have questions we encourage you to check out the [official SDV discord](https://stardewvalley.community/) for more help.

If you are struggling and would like PPJA to help you convert your pack please send me a [direct message on Nexus](https://www.nexusmods.com/users/26612284) with a link to your CFR pack and we'll see what we can do :) Once you do two or three patches it becomes much easier. Artisan Valley only took maybe an hour to convert.


