# laanp Mods

Compatible with Icarus Version: Rev. 2.1.7.118077 (Week: 104)
_______________________________________________________________________________________________________________________________________________________________________

Welcome to my collection of mods for Icarus: First Cohort. Below will be listed the various mods and a description of what they adjust. 
RECOMMENDED: Download the [Icarus Mod Manager by Jim72](https://github.com/Jimk72/Icarus_Software). It will allow you to easily and conveniently install, remove, merge, and update any mods you use! Mods can be updated every week simply by updating the data folder and then updating the installed mods without the need to re-download versions of them. 

Visit the [Linkarus Discord community](https://discord.gg/linkarus-icarus-modding-936621749733302292) for news, help, and other stuff 
regarding the modding community for the game!

To download the *.pak file, click on "Latest" Release button to the right of this page.

## Mods Available:

### laanp-Combined_QOL_v1_w104_P.pak
- Combines Quality-Of-Life mods(laanp) with others... CustomOptions(Jimk72), Teleporter(Jimk72) and Clear_Photo_Lens(JimK72)
- Check out the [Readme](https://github.com/laanp/Icarus_Mods_Separated/blob/main/laanp-Combined_QOL_Readme.md) for all the details.

### laanp-BuildersDream_v1_w104_P.pak
- Combines laanp-Combined_QOL + laanp_FreeBuild with a bunch of new features!:
- Check out the [Readme](https://github.com/laanp/Icarus_Mods_Separated/blob/main/laanp-BuildersDream_Readme.md) for all the details.

### laanp-StacksAndKits_v1_w104_P.pak
- A more natural Icarus experience, with a minimized kit set:
  - Player levels shows actual, beyond 60
  - Added new Workshop menu item called "Pete's Kits" - Which contains the following:
    - "Pete's Basic Starter Kit" (includes advanced tools, and a bedroll)
    - "Pete's All Seeds Farming Packets" - All the seeds in the game
    - "Pete's Promethius Kit" - containing the following:
      - (100) Frozen Ore
      - (100) Clay
      - (100) Obsidian
      - (100) Scoria
      - (100) Crystallized Miasma

### laanp-WorkshopFree_v1_w104_P.pak
- All items in the Workshop are free. Go crazy!

### laanp-PetesResourceKiller_v1_w104_P.pak
- Envirosuit module to enable 100% of the time, 1-hit resource gathering for trees, rocks & ores.
- Inspired by DexterMod's "One_Hit_Wonder" mod. 
- "Pete's Resource Killer" revises the Workshop Animal Healthbar module - When placed in aux. slot of suit, activates 100% chance of 1-hit resource gathering for trees, rocks & ores.
- Simply remove the module from your envirosuit auxilliary slot, to neutralize the effects and chop trees or mine normally.
- Make sure you have "Seasoned Logsman" talent unlocked, otherwise you'll end up spending all your time picking up wood, instead of it automatically going into your inverntory!

### laanp-KeepTheTrees_v1_w104_P.pak
- Stops trees from falling down in a wind storm and from catching on fire due to lightning strikes

### laanp-NoTreeLightningFires_v1_w104_P.pak
- Stops trees from catching on fire due to lightning strikes

### laanp-NoWindFallenTrees_v1_w104_P.pak
- Stops trees from falling down in a wind storm

### laanp-NoCaveWorms_v1_w104_P.pak
- Removes Cave Worms from spawning on all prospects including Missions & Open Worlds

### laanp-NoCaveWormsOW_v1_w104_P.pak
- Removes Cave Worms from spawning on Open World propsects only (Olympus & Styx Maps).

### laanp-NoFreezerIce_v1_w104_P.pak
- Stops ice from accumulating in the Deep Freeze (freezer)

### laanp-NoKeas_v1_w104_P.pak
- Disables spawning of Keas (big parrot-like birds)
- On some maps and in some of your building locations, Keas will spawn either directly in, or under base structures (especially when building higher bases).
  This can be quite annoying when building, this mod removes them from the maps entirely.

### laanp-NoWeather_v1_w104_P.pak
- Removes all weather from the game.
- Not compatible with JimK72's Icarus Mod Manager program, or other weather mods.  Just install the pak file directly into your mods folder.
- Can be used with all other mods, as long as they do not modify any of the weather json files.

### laanp-NoWaterWheelJunk_v1_w104_P.pak
- Water wheels no longer accumulate junk.

### laanp-RealLevels_v1_w104_P.pak
- Shows character true level based on experience points.
- Standard game will cap your level display at 60, and this mod will unlock it. 

### laanp-LargerDropshipSlots_v1_w104_P.pak
- Dropship cargo slots increase from 15 - 30 

### laanp-FreeBuild_v1_w104_P.pak
- Everything is free to build at all benches.
- Some things to watch:
  - Benches that auto craft items still need at least one item to start crafting - they will continue to craft until all slots are full
    for the first available recipe item in the bench inventory.

### laanp-MXC_CanUpgrade80k_v1_w104_P.pak
- Upgrades Workshop MXC Fuel Cannister to 80K pre-filled fuel 

### laanp-RespawnResourcesOW_v1_w104_P.pak
- Resets all Open World resources (Olympus, Styx, Promethius).  Use this mod whenever you want to reset your mines, nodes, trees, rocks.
- How To Use:
   - Install as per any mod (refer to Installation Details below)
   - Restart the game, load your open world prospect, all resources should have respawned, wait a save cycle, exit the game, then 
      delete this mod Pak file from the \mods directory.  Now you can restart the game and play with all resources replenished!
      Great for refreshing all those burnt trees, and refilling the mines. - Think of the Thumper without the worms! 

_______________________________________________________________________________________________________________________________________________________________________


## Installation Details

### Client (Local) machine:
Make sure Icarus has been shutdown, 
Place all your mod files (*.pak) in the game mods folder located here:

(drive):\Program Files (x86)\Steam\steamapps\common\Icarus\Icarus\Content\Paks\mods

if the ...\mods directory does not exist, create it.

If you are playing multiplayer where one person is hosting, Use the exact same mods
on everyone's PC, or else run the risk of weird stuff happening.
Usually the hosting player settings/mods will override anything running on the local client machine(s), but match the mods to stay out of trouble.

### Dedicated Server machine:
Make sure Icarus has been shutdown, 
Place all your mod files (*.pak) in the dedicated server game mods folder located here:

(drive):\<IcarusServerFolder>\Icarus\Content\Paks\mods

NOTE - Replace (drive):\<IcarusServerFolder>\ with the applicable location you installed your Icarus Dedicated Server app.

if the ...\mods directory does not exist, create it.

Use the exact same mods on both server and client machine or else run the risk of weird stuff happening.
Usually the server settings/mods will override anything running on the local client machine(s), but match the mods to stay out of trouble.


## Known Bugs/Issues/Notes - As of this current release.

### After a Game Update:
It is generally good practice to follow this procedure when the game goes through an update: 
   - After the files have been updated and patched, startup your Icarus game without any mods installed. 
   - Go into character selection, and view the talent/tech trees, then exit the game completely.  
   - Now install the new mods compatible with the week# and play the game.

### Custom Options Interface:
- "Deactivate Cave Worms" only works in single player client mode, Does not work on Dedicated Server.
- "Extinguish Fire" - Does not seem to work on forest fires in both single player & Dedicated Server
- "Clear Foliage" - Don't panic if you accidentally hit this and all your local flora is gone.  It only lasts for your current session.

### Teleporter:  
There is a known issue where ocassionally, after you teleport back to a saved destination when you walk over the teleport pad, you will teleport 
and the screen will become pitch black.  Just activate the remote on your hotbar (remember the key), and teleport back to the teleport pad.  
The screen should correct itself, then step off the pad and walk back over it to retry the teleport to the saved location.  
It will usually work the 2nd time you try. You'll also sometimes be teleported under the graphics mesh, just move around a bit and you will pop back up to the surface. 
If it still doesn't correct itself, hit ESC and click on the "Unstuck" menu option.

### "Pete's Resource Killer"
If you are using "Pete's Resource Killer" module (1 hit for tree, rocks and ore gathering) - it goes without saying if you are chopping a tree
with your axe, and do not have the Talent "Seasoned Logsman" - the one that auto picks up your wood, you'll end up with wood pieces all over
the place and not in your inventory!  This is expected behaviour.

### Equipment Retrieval
None of the unbundled equipment will come back with you after you leave the prospect via dropship. 
You need to purchase the kits at the Workshop, before launching any mission, Open World, or Outpost. 

## Youtube Links on Overview & How To Use:
- [Icarus - Quality of Life Mod Series - Part 1 - Download & Installation](https://youtu.be/5_hZUJ0OVdQ)
- [Icarus - Quality of Life Mod Series - Part 2 - Workshop Kits](https://youtu.be/2nrqFBvmzPc)
- [Icarus - Quality of Life Mod Series - Part 3 - Teleporter, Custom Options & Clear Lens Photo Mode](https://youtu.be/Cw6RRcEYQ6c)

## laanp_mod_compatibility_matrix.pdf

### How to use this matrix:
- Scan for your mod name in leftmost column and note the marked columns to the right showing associated json files that are affected. If any other mod is affecting the same file, then those mods are not compatible with the mod you have selected.

### For example:
- I scan for "laanp_LargerDropShipSlots" in leftmost column, and look across to the marked column of the json file affected.  In this case "D_InventoryInfo.json" is being affected.  But I also observe that my main "laanp-Combined_QOL_v1_w82" mod is also affecting this file, so the 2 mods are not compatible running together.  

## Disclaimer
I have been playing with these mods for quite some time now, with no problems... having said that:
- Backup and save all user data before installing or using any mods.
- Use at your own risk.
- This mod was designed as standalone, and may not be compatible with other mods.
- Ensure you are running the latest version of this mod with the latest version of Icarus.  Hint: the _w77_ in the mod file name means mod is compatible 
    with Week 77 Icarus release.  The _v1...2 etc in the mod file name refers to mod enhancements or fixes within the same week release. 
- This mod changes storage cabinets & bench inventory slot sizes.  
   If you fill all slots in these benches/storage cabinets on a prospect and return to it without these mods running, you will lose
   all those items in those additional slots. 
- Feel free to drop me any ideas for mod changes/suggestions.
- Feel free to re-distribute this mod provided recipients are directed to this Readme for mod credits and are aware of this Disclaimer and Known Bugs
- Feel free to unpack and reassemble with your modding tools, but if repacking and distributing, remove my "laanp" name from any distribution material,
   and make sure you acknowledge credit to any contributing modders.

## How To Contact Me:

- Discord: laanp
- Youtube Channel: [Icarus - First Cohort - BaseBuilding](https://www.youtube.com/channel/UCQWq0BjD4mnUkAZgRwwigNQ) 

Enjoy Prospectors!

































