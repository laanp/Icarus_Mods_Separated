# laanp Mods

Compatible with Icarus Version: Rev. 1.3.6.113408 (Week: 84)
_______________________________________________________________________________________________________________________________________________________________________

Welcome to my collection of mods for Icarus: First Cohort. Below will be listed the various mods and a description of what they adjust. 
RECOMMENDED: Download the [Icarus Mod Manager by Jim72](https://github.com/Jimk72/Icarus_Software). It will allow you to easily and conveniently install, remove, merge, and update any mods you use! Mods can be updated every week simply by updating the data folder and then updating the installed mods without the need to re-download versions of them. 

Visit the [Linkarus Discord community](https://discord.gg/linkarus-icarus-modding-936621749733302292) for news, help, and other stuff 
regarding the modding community for the game!

To download the *.pak file or *.EXMOD file, click on "Latest" Release button to the right of this page.

## Mods Available:

### laanp-Combined_QOL_v1_w84_P.pak
- Combines Quality-Of-Life mods(laanp) with others... CustomOptions(Jimk72), Teleporter(Jimk72) and Clear_Photo_Lens(JimK72)
- Check out the [Readme](https://github.com/laanp/Icarus_Mods_Separated/blob/main/laanp-Combined_QOL_Readme.md) for all the details.

### laanp-NoWeather_v1_w84_P.pak
- Removes all weather from the game.
- Not compatible with JimK72's Icarus Mod Manager program, or other weather mods.  Just install the pak file directly into your mods folder.
- Can be used with all other mods, as long as they do not modify any of the weather json files.

### laanp-LargerDropshipSlots_v1_w84_P.pak
- Dropship cargo slots increase from 15 - 30 

### laanp-FreeBuild_v1_w84_P.pak
- Everything is free to build at all benches.
- Some notes on this one:
  - Benches that auto craft items still need at least one item  to start crafting - they will continue to craft until all slots are full
    for the first available recipe item in the bench inventory.
  - Fishing bench (fillet section) should not have Rotten Meat left in it - otherwise it will fill up with Rotten Meat Lures!

### laanp-BuildersDream_v2_w84_P.pak
- Combines laanp-Combined_QOL + laanp_FreeBuild with a few adjustments:
   - Removes temperature effects on player
   - Modifies Workshop MXC Furnace to smelt everything, faster, and allows outdoor placement
   - Mortar & Pestle is immune to weather effects
   - Changes Workshop mod kit item "Pete's Starter Cabin Kit" to include 3 x modified MXC Furnaces (instead of 2 x Stone Furnaces)
   - Adds Workshop Item "Pete's Circular Construction Set" - Nice kit with lots of material for building a circular structure
   - Adds Workshop Item "Pete's Fishing Kit" - Nice kit with a Rod, Tackle box, Trap and all the lures.
   - Player can now directly craft Oxite, Coal & Salt from player crafting menu
   - Overall levelling is much faster, and mining Stone now levels up a character EXTREMELY fast! - This is to facilitate starting a new character and getting him up over level 30 quickly, to unlock everything to get to building.

### laanp-RespawnResourcesOW_v1_w84_P.pak
- Resets all Open World resources.  One time mod to use and reset your mines, nodes, trees, rocks.
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
### Custom Options Interface:
- "Deactivate Cave Worms" only works in single player client mode, Does not work on Dedicated Server.
- "Extinguish Fire" - Does not seem to work on forest fires in both single player & Dedicated Server
- "Clear Foliage" - Don't panic if you accidentally hit this and all your local flora is gone.  It only lasts for your current session.

### Teleporter:  
There is a known issue where ocassionally, after you teleport back to a saved destination when you walk over the teleport pad, you will teleport 
and the screen will become pitch black.  Just activate the remote on your hotbar (remember the key), and teleport back to the teleport pad.  
The screen should correct itself, then step off the pad and walk back over it to retry the teleport to the saved location.  
It will usually work the 2nd time you try.

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







































































































































































































