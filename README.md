# README

This is a thorough guide about fixing and enhancing _Fallout 3 Game of the Year Edition_, that is, _Fallout 3_ and all its DLCs. For now, this is a work in progress, as I am focusing on the contents first and on the layout later.

Take a look at the file `Modding never changes.md`. That is the main guide file, and it will be used to generate different final products (HTML, PDF, etc.).

### Changelog

**(v0.25) [06/09/2016] Rewrite complete up to 4.3.2.**

Well, this has been a hell of a task.

After finishing chapter 4.2, I started with 4.3.1, about FWE. But I made _three_ mistakes.

1. I didn't read BenWah's advice about creating a single file with the three available files for FWE in Nexus, provided you where using NMM instead of FOMOD (as I am doing). NMM doesn't install FWE the right way unless you merge the files first and foremost. As a collateral result, I discovered Xuul's videos, which have been **VERY** helpful.
2. I installed _Improved Sound FX v1\_3_ before FWE, and I didn't know, at the time, that these two mods collide. And, maybe due to NMM corruption (that's the third point), this simple fact fucked up the installation of FWE.
3. My copy of NMM was corrupted. I don't know why, but the file which keeps track of the installed files per mod (thus, using them to detect overlaps), located in `%NMM_HOME%\Fallout3\Mods\VirtualInstall\VirtualModConfig.xml`, contained information about _deleted_ mods I was no longer using (or I hadn't installed yet). You can imagine the plethora of WTFs I expelled when my installed mods count didn't match with my active mods count.

In short, I had to start over again! However, several bonuses have been gained:

* I found a new mod to speed up the Pip-Boy animation ([_Faster Pipboy Faster_](http://www.nexusmods.com/newvegas/mods/35225/?)), so pulling it up is not excruciatingly slow.
* I fixed the green tint problem with high resolution maps using [_Shiloh DS - Clean Pipboy Screen_](http://www.nexusmods.com/newvegas/mods/36255/?) mod. The "Clean Pipboy Screen" feature in [_Better High Detail Map and Icons_](http://www.nexusmods.com/fallout3/mods/16898/?) only removes "old electronics" artifacts from the Pip-Boy screen, but it doesn't remove the green tint. Besides, with this mod the map fits perfectly within the bounds of the usable area, without need to tinker with configuration files.
* I relocated [_Improved Sound FX v1\_3_](http://www.nexusmods.com/fallout3/mods/627/?) after FWE, screwing up my functional approach to mod setup, but hey, you have to make sacrifices now and then.

Next stop: Mart Mutants Mod!

**(v0.24) [02/09/2016] Complete chapter 4.2 overhaul.**

I have completely rewritten chapter 4.2 about sound and music. Where we had just one mod, we have now six different mods, ranging from weapon sounds to new songs from radio stations scattered throughout the Wasteland. The sense of immersion has greatly improved with the contents of this chapter.

**(v0.23) [29/08/2016] Chapter 4.1 rewritten and updated.**

The chapter 4.1 (user interface) has been easier. Most of the pictures already had red boxes pointing out selected options/buttons. I have downscaled the screenshots anyway.

The biggest changes have been made in 4.1.5 (world map retexturing), because I finally managed to get rid of the green tint of the original map. The full-sized map of the mod is shown in all its colorful glory.

I have not used [_Color Hi-Detailed map and icons_](http://www.nexusmods.com/fallout3/mods/1789/?) because I thought the maps in that mod were high-resolution, but nope!

**(v0.22) [29/08/2016] Chapter 3 rewritten and updated.**

I have started the next iteration, with new mods. However, I am making the most of it by rescaling the images and correcting errors in the text.

The chapter 3 has been rewritten, with downscaled images (a lot less weight in the final file) and with a new section, 3.11, about removing unused objects from the game.

**(v0.21) [29/08/2016] New section about creating a merged patch.**

I have written a new chapter (6; I moved previous chapter 6 to number 7) about creating a merged patch with the mod stack you have installed to that point. It is an important final step in every mod installation we are going to do.

This is the final chapter in the first iteration (now it is, trust me). The next version will be about a new iteration.

**(v0.20) [25/08/2016] Fixed load order lists.**

I have added a few missing load order lists in the initial chapters. I have also highlighted the installed files in the lists that didn't have them highlighted (all load order lists previous to _Project Reality_).

**(v0.19) [24/08/2016] Section about people redesigned finished.**

At last!

Final chapter finished... Well, _almost_ final chapter. There are a few remaining loose ends to finish (a merged patch, highlighting of the installed files in each load order listing, etc.).

This chapter is about people reanimated (new and more natural animations) and redesigned (a huge overhaul of face meshes all around the game). And that's it. This is the game we are going to play.

However, there are certain mods that I would like to include in the following rehearshal. I have wrote them down in a separate sheet in `Mods installed.ods`. I will consider the contents finished then.

**(v0.18) [21/08/2016] Section about lighting finished.**

Added a new section about lighting, both in interiors and exteriors, setting a scarier mood in the nights. These mods fit perfectly with darker nights from _Project Reality_.

**(v0.17) [20/08/2016] Section about new visuals finished.**

Added a new section about visuals (5.4), covering ground from new textures to increased flora, going through crystal clear waters and a cleaned-up environment.

Almost there!

**(v0.16) [15/08/2016] Section about vision control finished.**

Added a new section about vision control (5.3), with four mods which allow to change the way we see the Wasteland.

The final three chapters (5.4, 5.5 and 5.6) are on their way. I have planned the install order, so I have added the chapter stubs, writing down the remaining mods to install.

**(v0.15) [07/08/2016] Section about Project Reality finished.**

Added a new section about Project Reality, a mod that changes the way the Wasteland looks (much better, in my opinion), and adds dynamic weather and much darker (and terrifying) nights.

**(v0.14) [07/08/2016] Section about night sky enhancement finished.**

Finally!

I have started the final big chapter of the book. This big chapter (5) deals with graphic-enhancement mods.

The first chapter (5.1) changes the detail and brightness of the night sky with two simple mods.

**(v0.13) [07/08/2016] Section about achievement list finished.**

I have added a small section about a mod that creates a list of all your fulfilled achievements in the game, with retroactive effect.

There are no screenshots, though, because I am not getting the option in my PipBoy, neither in my regulator, nor in my vault dweller saved games.

If I don't get this mod to work in a fresh playthrough, I will remove this chapter.

**(v0.12) [07/08/2016] Section about Advanced Gear set finished.**

I have included a new section (4.4.2) about Gopher's Advanced Recon set, with new armor, trap detector, nightvision, thermal vision and range finder.

Besides, I have rearranged section 4, moving the expanded content to its own section (4.4.1), and planning a new section about a revamped achievement log (4.4.3).

**(v0.11) [06/08/2016] Section about expanded content revisited.**

I have made a few minor adjustments to the section 4.4 (former 4.3.4), about expanded content. The only remarkable change is the load order.

We are ready to change the way the game looks now.

On a side note, it's a bit difficult to write a guide like this with a cat craving for attention in your lap.

**(v0.10) [26/07/2016] Section about weapons finished.**

At last!

I have finished the section about weapons system revamp (WMK, EVE and RH_IronSights). The game runs without crashes (apparently), but I have no installed the compability patch among FWE, EVE and MMM, because we are going to install Project Beauty, and there is a combo patch for all of them.

The end is nigh!

**(v0.9) [24/07/2016] Section about MMM reworked.**

I have rewritten the section about _Martigen's Mutant Mod_, using one of the merged patches from Paradox Ignition. I am going to use these patches for WMK, EVE and RH_IronSights also, applying a _Blackened_ compatibility patch when finished.

**(v0.8) [24/07/2016] Section about audio overhaul finished.**

New section (4.2. Lend me your ears) about audio overhaul of the game. I have added a short chapter (4.1.7. Shed some light here, please) about Pip-Boy's lamplight revamp.

However, the big thing here is that I had to start modding the game from scratch, because I realized I had to use Paradox's The Mergers patches (along with Blackened compatibility patches) to the next main series of mods (FWE, MMM, EVE and WMK).

I didn't feel comfortable rolling back some mods, and my 7 GB backup copy didn't work because I didn't copy metadata from NMM describing the actual installed mods, so, I had no other choice.

**(v0.7) [10/07/2016] Section about new content finished.**

New section (4.2.3. Expanding your world) about new content mods (_Alton, IL_, _Arefu Expanded_ and _Mothership Zeta Crew_).

**(v0.6) [10/07/2016] Section about _Martigen's Mutant Mod_ finished.**

New section (4.2.2. Fraternizing with the neighborhood) about _Martigen's Mutant Mod_, a mod that adds a lot of new creatures and encounter/fight mechanics to the game.

**(v0.5) [04/07/2016] Corrections and additions.**

Corrections and additions in sections 4.1.3 and 4.2.1.

**(v0.4) [29/06/2016] Section about _Fallout 3 Wanderers Edition_ finished.**
The section 4.2.1 is finished, covering the installation of FWE, letting us play a completely different game, harsher and more challenging.

**(v0.3) [26/06/2016] Section about UI finished.**

The section 4.1 is finished, covering from the HUD to the Pip-Boy. The game should look slightly better now, but not in a blowing-off-your-head way.

**(v0.2) [25/06/2016] Rough draft of the section about UI.**

Two sections finished about improving how your user interface looks (sections 4.1.1 and 4.1.2).

**(v0.1) [24/06/2016] First chapter finished.**

The first chapter is about fixing the game. At the end of the chapter, you will have a fully patched and (mostly) flawless game to play with. The content, visuals and mechanics of the game are not altered in this stage.