# Modding... Modding never changes




## Table of contents

* [1. Introduction](#introduction)
* [2. The tools we need](#toolsWeNeed)
* [3. Fixing the game](#fixingGame)
	- [3.1. Install the game](#installGame)
	- [3.2. Disable Games for Windows Live](#disableGFWL)
	- [3.3. Patching the game](#patchingGame)
	- [3.4. Cleaning up the master files](#cleaningMasterFiles)
	- [3.5. Enabling the console](#enablingConsole)
	- [3.6. Enabling access to 4+ GB of memory](#largeAddressAware)
	- [3.7. _Fallout 3_ Script Extender](#fose)
	- [3.8. Getting rid of stutter](#gettingRidStutter)
	- [3.9. Fake full-screen mode](#fakeFullScreen)
	- [3.10. Saving games the right way](#casm)
	- [3.11. Adopt an useless rock today!](#adoptUselessRock)
* [4. Enhancing the game](#enhancingGame)
	- [4.1. Improving the user interface](#improvingUserInterface)
		+ [4.1.1. Building the basement](#buildingBasement)
		+ [4.1.2. Face-washing the HUD](#faceWashingHUD)
		+ [4.1.3. Rearranging things](#rearrangingThings)
		+ [4.1.3. Seeing things just when you need to](#seeingThingsWhenNeeded)
		+ [4.1.4. Cleaning up your faithful companion](#retexturingPipBoy)
		+ [4.1.5. You don't want to ask for directions](#betterMap)
		+ [4.1.6. No more dots](#noMoreDots)
		+ [4.1.7. Shed some light here, please](#shedSomeLight)
	- [4.2. Lend me your ears](#lendMeYourEars)
		+ [4.2.1. Hearing the nukes fly in high quality](#hearingNukesFly)
		+ [4.2.2. Those crickets are driving me mad](#thoseCrickets)
		+ [4.2.3. A soundtrack for your lonely Wasteland nights](#radioStations)
	- [4.3. Playing the bad-ass way](#playingBadAss)
		+ [4.3.1. _Ad astra per aspera_](#adAstraPerAspera)
		+ [4.3.2. A sound for Chekhov's gun](#checkhovsGun)
		+ [4.3.3. Fraternizing with the neighborhood](#fraternizingNeighborhood)
		+ [4.3.4. We need more firepower!](#weNeedMoreFirepower)
	- [4.4. Expanding your world](#expandingYourWorld)
		+ [4.4.1. _Hic sunt dracones_](#hicSuntDracones)
		+ [4.4.2. Gear for a fallen brother](#gearFallenBrother)
		+ [4.4.3. For the achievement junkie in you](#achievementJunkie)
	- [4.5. So you want to take over the world, uh?](#takeOverTheWorkd)
* [5. Unveiling the real Wasteland](#unveilingRealWasteland)
	- [5.1. She walks in beauty, like the night of cloudless climes and starry skies](#sheWalksInBeauty)
	- [5.2. The Nuclear Holocaust like you have never seen before](#uncannyNuclearHolocaust)
	- [5.3. Everything depends on the point of view](#pointOfView)
	- [5.4. A beautiful skin](#beautifulSkin)
	- [5.5. Let there be light!](#letThereBeLight)
	- [5.6. I don't like your face](#dontLikeYourFace)
* [6. Wrapping up](#wrappingUp)
* [7. Resources](#resources)
	* [7.1. Tools](#tools)
	* [7.2. Guides](#guides)
	* [7.3. Mods](#mods)
	* [7.4. Videos](#videos)




## <a id="introduction"></a>1. Introduction

We, human beings, have a strange knack for imagining Doomsday. We like to depict our planet devastated by plagues, war (either biological or nuclear), alien attacks or all together at the same time.

One of the videogames that best shows how our world could be after a nuclear holocaust is _Fallout 3_. And [I'm not the only one](https://warisboring.com/why-fallout-is-the-best-nuclear-war-story-ever-told-5910918d28e4) with that feeling.

However, if you have been around the videogame scene for a while, you will know that _Fallout 3_ can be completely enhanced using _mods_... Well, that is a complete understatement, as you could play a whole different game with the appropriate mods. Or you could break the game. That's the tricky part.

Getting right to the point, vanilla _Fallout 3_ sucks in many different ways. You cannot even run the game if your box uses Windows 7 or higher. A lot of tinkering has to be done for the game to run flawlessly.

There is an awesome [guide to fix the game in order to run under modern versions of Windows](http://steamcommunity.com/sharedfiles/filedetails/id=149946772), written by [BenWah](http://steamcommunity.com/id/benwaa), which I intend to follow. And there are [a hell of a lot of videos by Gopher](https://www.youtube.com/channel/UC1CSCMwaDubQ4rcYCpX40Eg) with the best _Fallout 3_ mods your money can buy (well, sort of). Give credit when credit is due, you know.

So, there is no original work here, just an extended guide to put things into perspective. And this perspective is divided into two parts:

1. The firs part (chapters [2](#toolsWeNeed) and [3](#fixingGame)) is about _fixing_ the game. At the end of these chapters, you will have a flawless _Fallout 3_ game, running smoothly, with no CTD (_Crashes to Desktop_ in jargon), but it will be a vanilla game, at least content, graphics and audio-wise. No changes will be made to the story or the way you perceive the Wasteland.
2. The second part (chapters [4](#enhancingGame), [5](#unveilingRealWasteland) and [6](#wrappingUp)) is about _enhancing_ the game. This is pretty based on personal taste, so feel free to ignore me (too bad) or, even better, modify this guide to your heart's content. I have picked the mods I like most, but your mileage may vary.
3. The final part (chapter [7](#resources)) is about resources used in the making of this book (videos, guides, etc.).

_I **DO** want to set the world on fire..._




## <a id="toolsWeNeed"></a>2. The tools we need

First and foremost, we need _Fallout 3 Game Of The Year Edition_ installed. This guide refers to the Steam version of the game.

We will need three additional tools to get the job done:

* [Nexus Mod Manager](http://www.nexusmods.com/games/mods/modmanager/). This is the tool of choice when it comes to keep all your mods organized and up-to-date.
* [LOOT](https://loot.github.io/). Installing mods on Bethesda games can be a pain in the ass, especially if you try to install a lot of possibly-colliding mods. This tool keeps the load order straight.
* [FO3Edit](http://www.nexusmods.com/fallout3/mods/637/). _Fallout 3_ itself comes out-of-the-box with certain errors in the main and DLC files, and this tool comes in handy to correct them. Besides, this is **THE** tool to [create a merged patch](#wrappingUp) to run the game with an absurd amount of mods.

Install them first and we are good to go.




## <a id="fixingGame"></a>3. Fixing the game

At the end of this section, you will have a version of _Fallout 3 Game of the Year Edition_ that:

* Runs flawlessly (well, almost).
* Is patched to the max, with most silly (and not-so-silly) errors corrected.
* Takes advantage of your system memory.
* Has no (or little) microstutter.
* Runs in windowed mode, faking full-screen.
* Has a clean set of data files, including a merged patch to further ensure compatibility among them.
* Creates saved games automatically and frequently, so that you always have means to recover from a disaster.
* Has a better performance by getting rid of zillions of unused objects (like tiny rocks) which plague the game.



### <a id="installGame"></a>3.1. Install the game

Pretty much straightforward, uh? Well, no. You need to run the game at least once to create the `.ini` files we will tinker with.

Again: you **MUST** run the game at least once in order to fix it.

The launcher dutifully informs you that video hardware is about to be detected, thus setting up the configuration for you.

![Fallout 3 video hardware detection](Images/Fallout%203%20video%20hardware%20detection.png)

Lucky me, my video card is up to the task (however, you don't want to know the specs of my box; no need to cry).

![High Quality settings set](Images/HQ%20settings%20set.png)

And here we go! This is the launcher in all its greenish glory.

![Fallout 3 launcher](Images/Fallout%203%20launcher.png)

Finally, click on _Play_, and enjoy the view.

![Fallout 3 main menu](Images/Fallout%203%20main%20menu.png)

Bear in mind that no matter how hard you pray or curse, this is as far as the game gets running in any version of Windows higher than XP. But this is all we need, for now. Just click on _Quit_ and check this files and folders under `[%USERPROFILE%\Documents\My Games\Fallout3]`:

* `[Saves]`
* `FALLOUT3.INI`
* `FalloutPrefs.ini`
* `RendererInfo.txt`



### <a id="disableGFWL"></a>3.2. Disable Games for Windows Live

In BenWah's guide you can either update your Games for Windows Live (GFWL for short) installation, or disable it. Unless it's vital to you, I recommend disabling GFWL, just in case.

To disable GFWL, you need to download and run [Games for Windows LIVE disabler](http://www.nexusmods.com/fallout3/mods/1086/).

**DO NOT** use Nexus Mod Manager (NMM for short) to download this tool. Download it manually instead.

If you get a warning about absent `FALLOUT.INI`, please run the game once (I told you).

![GFWL Disabler error](Images/GFWL%20Disabler%20error.png)

In the following window, just click on _Disable G4WL_.

![GFWL Disabler](Images/GFWL%20Disabler.png)

Of course, you want to remove GFWL buttons in the game.

![GFWL Remove Fallout 3 buttons](Images/GFWL%20Remove%20Fallout%203%20buttons.png)

We have our first patch!

![GFWL Disabled](Images/GFWL%20Disabled.png)

Notice the absent _LIVE_ option in the main menu screen:

![Fallout 3 main menu with no LIVE](Images/Fallout%203%20main%20menu%20with%20no%20LIVE.png)



### <a id="patchingGame"></a>3.3. Patching the game

_Fallout 3_ comes with a shitload of bugs, even after 5 DLC's. That is Bethesda's hallmark, but people has come to, if not love these bugs, at least consider them like you would consider your old grandpa pissing in the punch bowl on Christmas Eve. Slightly disgusting but, nevertheless, adorable.

Thanks to the efforts of BenWah and other people around, we have the [Unofficial Fallout 3 Patch](http://www.nexusmods.com/fallout3/mods/19122/), with a huge list of fixes and improvements.

1. Download manually (not with NMM) the file _Updated\_Unofficial\_Fallout3\_Patch_.
2. Run the file `Updated_Unofficial_Fallout3_Patch-19122-2-2.exe` (or something like that) to show the welcome window.
![UF3P Welcome window](Images/Unofficial%20Fallout%203%20Patch%201.png)
3. Accept the license agreement.
![UF3P License agreement](Images/Unofficial%20Fallout%203%20Patch%202.png)
4. The program shows the patch notes. These are important, as they clearly point out that you should have the GOTY version of the game, with all DLC to take full advantage of the patch.
![UF3P Patch notes](Images/Unofficial%20Fallout%203%20Patch%203.png)
5. Choose the location of _Fallout 3_. The program usually picks the correct folder right off the bat.
![UF3P Fallout 3 location](Images/Unofficial%20Fallout%203%20Patch%204.png)
6. Select the desired patch components. You should keep the default settings (all DLC and several minor but useful fixes).
![UF3P Component selection](Images/Unofficial%20Fallout%203%20Patch%205.png)
7. Choose the menu entry location in the Start Menu folder.
![UF3P Start menu folder](Images/Unofficial%20Fallout%203%20Patch%206.png)
8. The program shows the installation summary. Just press _Install_.
![UF3P Installation summary](Images/Unofficial%20Fallout%203%20Patch%207.png)
9. You should then see this window to be happy. Otherwise, you should be very, very sad (really).
![UF3P Status check](Images/Unofficial%20Fallout%203%20Patch%208.png)
10. Here we go! The installation takes a while, because the patch moves around a lot of files.
![UF3P Installation progress](Images/Unofficial%20Fallout%203%20Patch%209.png)
11. When the installation finishes, the program shows a dialog with some techno-gibberish speak. Fear not! _Fallout 3_ [crashes if running in a box with multiple cores](http://www.sevenforums.com/gaming/20199-fallout-3-windows-7-w-quad-core.html), but the patch fixes the configuration options automatically for you. Click _Yes_, of course.
![UF3P Multicore fix](Images/Unofficial%20Fallout%203%20Patch%2010.png)
12. Happy ending! The installation is finished.
![UF3P Happy ending](Images/Unofficial%20Fallout%203%20Patch%2011.png)
13. Delete the executable file and move on with your life.

There is one final step to ensure that the patch is loaded in the proper place, at the bottom of the data files.

Each data file can come in two flavors: `.esm` for master files or `.esp` for secondary (patch) files. The DLCs themselves are `.esm` files.

This is a good time to check the load order of the game data files, so fire up LOOT to see what is happening under the hood. On a side note, Gopher has published two videos, one explaining [what is 'load order' and why it is important](https://www.youtube.com/watch?v=YzsBKYUrcbE) (20:00), and other explaining [what is LOOT and how to put it to good use](https://www.youtube.com/watch?v=SzoyWugzZAw) (13:59).

![LOOT first run after UF3P](Images/LOOT%20first%20run%20after%20UF3P.png)

After clicking on the sort icon, the program proposes the proper load order, meanwhile detecting data inconsistencies.

![LOOT after sorting](Images/LOOT%20after%20sorting.png)

This should be your load order by now:

* `Fallout 3.esm`
* `Anchorage.esm`
* `ThePitt.esm`
* `BrokenSteel.esm`
* `PointLookout.esm`
* `Zeta.esm`
* **`Unofficial Fallout 3 Patch.esm`**

You might be surprised to check that there are inconsistencies in the main DLC files, like `Anchorage.esm` (master file for _Operation Anchorage_ DLC). As we said, Bethesda is not known for releasing solid, fully tested programs. We'll address that later.

For now, just click on _Apply_ to put the unofficial patch at the bottom of the load order.

You should test the game right now. If everything went OK, you should be able to play the game.

![Fallout 3 first run](Images/Fallout%203%20first%20run.png)

Yippee ki-yay, motherfucker!



### <a id="cleaningMasterFiles"></a>3.4. Cleaning up the master files

Sure, you could play the game right now if you want. You would be playing a crippled, prone to crash game, but hey, if that's your thing...

We have miles to go before we sleep, though. Cheers for the brave who don't take second best!

As we saw earlier, the DLC data files themselves are somewhat _dirty_. This is what LOOT has to say about them (ITM means "Identical to Master"):

* `Anchorage.esm`: Contains 54 ITM records and 10 deleted references.
* `ThePitt.esm`: Contains 40 ITM records and 5 deleted navmeshes.
* `BrokenSteel.esm`: Contains 275 ITM records, 34 deleted references and 12 deleted navmeshes.
* `PointLookout.esm`: Contains 21 ITM records.
* `Zeta.esm`: Contains 15 ITM records.

The only clean file in your load order is `Unofficial Fallout 3 Patch.esm`, as expected. No wonder, this is a huge patch that fixes the game and all its DLCs.

In every single case, LOOT has a suggestion: clean with [FO3Edit](http://www.nexusmods.com/fallout3/mods/637/).

FO3Edit is an utility aimed at mod creators and users both, weighting more on the first group. Gopher has a fantastic video explaining [how to use TES5Edit (the _Skyrim_ version of the tool) to clean your master files](https://www.youtube.com/watch?v=fw3g_N1jcZQ) (13:24). You should left what you were doing right now and watch the video. I'll wait.

We are going to clean the master files, one by one. This guide about [cleaning files with TES5Edit](http://www.creationkit.com/index.php?title=TES5Edit_Cleaning_Guide_-_TES5Edit) comes in handy, but ignore it if you just want the heart of the issue.

I will show the instructions to clean one of the files, considering the rest are treated all the same.

1. Fire up FO3Edit. The tool does a good job detecting _Fallout 3_ data folder, thus showing all the data files we are using so far.
![FO3Edit master-plugin selection](Images/FO3Edit%20master-plugin%20selection.png)
2. Right-click on the floating window and select _Select none_. We are going to choose the files to clean, one by one.
![FO3Edit selecting none](Images/FO3Edit%20selecting%20none.png)
3. Now select the following files and click _Ok_:
	* `Fallout3.esm`.
	* The data file you are going to clean (for example, `Anchorage.esm`).
![FO3Edit selecting files](Images/FO3Edit%20selecting%20files.png)
4. After a while, depending of the size of the data file, the tool finishes loading the data, plus the `Fallout3.exe` executable itself. Wait for the message "Background Loader: finished" to appear in the _Messages_ panel.
![FO3Edit file loaded](Images/FO3Edit%20file%20loaded.png)
5. Right-click on the `Anchorage.esm` node in the left panel tree and select _Apply filter for cleaning_.
![FO3Edit apply filter for cleaning](Images/FO3Edit%20apply%20filter%20for%20cleaning.png)
6. The filtering may take a little while, depending on how big and dirty the file is. When the filtering is completed, a line with the heading "[Filtering done]" appears in the _Messages_ panel. The tree in the left panel shows the files with fancy colors which you don't have to give a fuck, unless you want to delve deeper into the inner workings of the mods.
![FO3Edit after filtering](Images/FO3Edit%20after%20filtering.png)
7. First, we are going to remove ITM (_Identical to Master_) records. They are not going to crash the game, but they take up space, and trust me, when you get the I-am-going-to-install-every-fancy-mod-available spree, you will need as much space as you can get. Right-click on the `Anchorage.esm` node in the left panel tree and select _Remove "Identical to Master" records_.
![FO3Edit remove ITM records](Images/FO3Edit%20remove%20ITM%20records.png)
8. Every time you try to change a data file, a big warning appears. But, as seasoned hard-ass mod installers, we are sure as hell of what we are doing. Aren't we?
![FO3Edit warning](Images/FO3Edit%20warning.png)
9. After a little while, a message shows up in the _Messages_ panel, reporting 43696 records processed and 54 records removed (don't worry if the numbers don't match; your setup may be slightly different).
![FO3Edit ITM records deleted](Images/FO3Edit%20ITM%20records%20deleted.png)
10. Next, we are going to undelete and disable deleted references... Unlike ITM records, which can be considered mostly harmless, deleted references can (and will) fuck up your game, because they are references to objects that _are supposed to be in the game_, but they no longer are, _and no one has marked them as disabled_. So, any mod using a deleted but not disabled reference is going to eventually crash your system. We are talking serious shit here. To get rid of these nasty sons of a bitch, right click on the `Anchorage.esm` node in the left panel tree and select _Undelete and Disable References_.
![FO3Edit undelete and disable references](Images/FO3Edit%20undelete%20and%20disable%20references.png)
11. A bit of processing again, and we have another message in the right panel, reporting 43642 records processed and 10 undeleted records.
![FO3Edit after undeleting and disabling](Images/FO3Edit%20after%20undeleting%20and%20disabling.png)
12. Job done! We just need to save the modified data file. To do that, just click on the close button of the tool window. A pop-up window should appear with _just one file_, the one you have been tinkering with (`Anchorage.esm`, in this case). If more than one file is shown, press <kbd>ESC</kbd> or click on the close button and start over again, because you surely screwed up at some point in the process. Anyway, make sure that the option _Backup plugins_ is selected before clicking _Ok_.
![FO3Edit save changed files](Images/FO3Edit%20save%20changed%20files.png)

You have to repeat the process for each and every one of the aforementioned data files.

In case you wonder, FO3Edit creates a folder named `[FO3Edit Backups]` under `[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data]` where it stores backup copies of the mods we have modified.

Run LOOT to be sure that we have a clean, patched game now.

![LOOT after cleaning](Images/LOOT%20after%20cleaning.png)

And, of course, run the game just to be on the safe side.

![Fallout 3 first patched run](Images/Fallout%203%20first%20patched%20run.png)



### <a id="enablingConsole"></a>3.5. Enabling the console

The game console is not strictly necessary to fix the game, but it will come in handy to test the fixes we apply.

I am using the console to cheat my way out the Vault 101, because testing each new mod with a fresh start may be weary, to say the least.

Enabling the console means editing `FALLOUT3.INI` file in `[%USERPROFILE%\Documents\My Games\Fallout3]`, setting the following line, which should be enabled by default (make sure you make a backup copy first):

```INI
bAllowConsole=1
```

The actual key used to activate the console depends on the keyboard language layout you are using, but it should be to the left of the <kbd>1</kbd> key. In en-US keyboards it is bound to the tilde character <kbd>~</kbd>, but, for example, in the es-ES layout (Spanish), that key is bound to the numeral character <kbd>º</kbd>.

To test the console, start the game and press the corresponding key while in the main menu. A tiny vertical cursor will appear in the lower left corner of the screen. Run the following command:

```
GetDayOfWeek
```

The system should print something like:

```
GetDayOfWeek >> 5.00
```

![Fallout 3 testing the console](Images/Fallout%203%20testing%20the%20console.png)

There is no way to change the key assigned to the console, unless you install [_Console Key Binder_](http://www.nexusmods.com/fallout3/mods/2637/) mod. However, you should keep your mod stack to a minimum (says the guy who is creating a guide to install shy of 100 mods). If you want to install this mod nonetheless, you should have installed first _Fallout Script Extender_, which we will be covering in [a later section](#fose).

Finally, there is an exhaustive [list of console commands](http://www.tweakguides.com/Fallout3_11.html) in the awesome [_Fallout 3 Tweaking Guide_](http://www.tweakguides.com/Fallout3_1.html).



### <a id="largeAddressAware"></a>3.6. Enabling access to 4+ GB of memory

_Fallout 3_ does not use all the available memory it could have due to its 32 bits nature (the game was launched in 2008, you know). However, you can modify the game executable to take advantage of all the memory it can get.

Gopher explains the way to go with this video about [performance and stability in _Fallout 3_](https://www.youtube.com/watch?v=tONiXNbwSt0) (26:38) (the video touches several topics, but the one we are focusing on spans from the beginning to 08:55, give or take).

We don't want to clutter our system with unnecessary tools, so we are sticking with [Large Address Aware Enabler for _Fallout 3_](http://www.nexusmods.com/fallout3/mods/6510/).

1. Download the mod manually (not using NMM), and extract its contents in a location of your choice (`[%LAA_FOLDER%]`, for reference).
2. Create a backup of the file `Fallout3.exe` from `[%STEAM_HOME%\steamapps\common\Fallout 3 goty]`.
3. Copy the file `Fallout3.exe` to `[%LAA_FOLDER%]`.
4. Run `START.BAT` in `[%LAA_FOLDER%]`. A console window will appear, reporting that the patching is about to start. Press any key.
![LAA Enabler](Images/LAA%20Enabler%20reminder.png)
5. Several options are shown. We want to press <kbd>A</kbd> to add the LAA feature to _Fallout 3_ executable.
![LAA Enabler options](Images/LAA%20Enabler%20options.png)
6. LAA Enabler patches the executable and happily informs us about it. Press any key.
![LAA Enabler successful](Images/LAA%20Enabler%20successful.png)
7. The program goes back to the options window. Press <kbd>E</kbd> to exit.
8. Copy back `Fallout3.exe` to its original location.
9. Delete the folder `[%LAA_FOLDER%]` and its contents. Delete the ZIP file also. You won't need them anymore.

And that's really it. Now _Fallout 3_ is ready to handle more than 2 GB of RAM, improving stability.



### <a id="fose"></a>3.7. _Fallout 3_ Script Extender

If you ever want to install a single mod in _Fallout 3_, you will need [_Fallout Script Extender_](http://fose.silverlock.org/) (FOSE, for short).

Well... That's not exactly true, as there may be mods that does not make use of the capabilities provided by FOSE (we have been using a few, so far). But they will be a minority. And we will need this tool ahead the road.

As usual, Gopher has published a worth watching video about the [installation and use of FOSE](https://www.youtube.com/watch?v=QK_f4vHiutA) (10:07).

1. Download the latest version of FOSE ([1.2b2](http://fose.silverlock.org/download/fose_v1_2_beta2.7z) as of this writing). You should download the 7Z version, not the loader (`fose_v1_2_beta2.zip`).
2. Extract the contents of the archive into a folder of your choice, say `[%FOSE_FOLDER%]`.
3. Copy the contents of the folder `[%FOSE_FOLDER%]` to `[%STEAM_HOME%\steamapps\common\Fallout 3 goty]`, except the folder `[src]`, which contains FOSE source code.
4. Delete the folder `[%FOLSE_FOLDER%]` and its contents. Delete the ZIP file also.
5. Create a shortcut for the file `fose_loader.exe` in a location of your choice (e.g., your desktop).
6. Rename the shortcut to whatever name you feel comfortable with. I go with _Fallout 3_, because I keep the older shortcut, using the launcher, to configure the game, thus renaming it to _Fallout 3 (config)_.
![Fallout 3 launch shortcuts](Images/Fallout%203%20launch%20shortcuts.png)
7. If you, like me, think that the default shortcut icon is [Deathclaw](http://fallout.wikia.com/wiki/Deathclaw) shit, it might be worth considering an [alternate icon](http://www.iconarchive.com/show/mega-games-pack-23-icons-by-3xhumed/Fallout-3-new-1-icon.html). Download the `.ico` version and copy it to `[%STEAM_HOME%\steamapps\common\Fallout 3 goty]`.
8. Right-click on the shortcut icon and select _Properties_.
![Fallout 3 shortcut properties](Images/Fallout%203%20shortcut%20properties.png)
9. In the _Shortcut_ tab, select the option _Change icon..._.
![Fallout 3 shortcut change icon](Images/Fallout%203%20shortcut%20change%20icon.png)
10. The system dutifully informs you that `fose_loader.exe` (the executable the shortcut refers to) does not contain any available icon. Click _Ok_.
![Fallout 3 shortcut no default icon](Images/Fallout%203%20shortcut%20no%20default%20icon.png)
11. The system shows a floating window where you could select one of the shitty system default icons. Just click on _Browse_...
![Fallout 3 shortcut select icon](Images/Fallout%203%20shortcut%20select%20icon.png)
12. Select the `.ico` file you downloaded before and click _Open_.
![Fallout 3 shortcut open icon](Images/Fallout%203%20shortcut%20open%20icon.png)
13. Back to the icon selection window, click on _Ok_.
![Fallout 3 shortcut icon selected](Images/Fallout%203%20shortcut%20icon%20selected.png)
14. Back to the properties window, click on _Ok_.
![Fallout 3 shortcut properties final](Images/Fallout%203%20shortcut%20properties%20final.png)
15. _Et voila!_ We have now two great-looking icons to launch _Fallout 3_, one to configure it and the other to actually launch a mod-friendly version of the game.
![Fallout 3 launch shortcuts final](Images/Fallout%203%20launch%20shortcuts%20final.png)
16. We are going to test that FOSE is correctly installed, and for that, launch the game with the new shortcut. In the main menu screen, activate the console and write `GetFOSEVersion`. You should get something like `FOSE version: 1`.
![Fallout 3 FOSE installed](Images/Fallout%203%20FOSE%20installed.png)

FOSE provides a [whole new set of console commands](http://fose.silverlock.org/fose_command_doc.html) you can use, although they are not strictly necessary.



### <a id="gettingRidStutter"></a>3.8. Getting rid of stutter

_Fallout 3_ suffers from stuttering, this is, there are certain points in the game where the visuals are lacking in fluidity. Although this can be reduced by optimizing your system (updating your graphics driver to the top, unfragmenting the hard drive, and so on), there is still a micro-stuttering that can be perceived in lower-spec machines when framerate suddenly changes.

In the same video about [performance and stability](https://www.youtube.com/watch?v=tONiXNbwSt0) (26:38), Gopher talks about this problem, from minute 08:55 to 16:40, more or less. We are going to install our first mod (apart from the unofficial patch), and for this, we are going to need [_Nexus Mod Manager_](http://www.nexusmods.com/games/mods/modmanager/) or NMM. This is the tool that allows to keep track of the installed mods, along with their updates.

Provided that you have installed NMM:

1. Run NMM. If this is the first time you do so, NMM searches for the games it knows of, modding-wise. In this context, we are only interested in _Fallout 3_, so as soon as NMM finds it, we should confirm the location (with the green tick mark under the name of the game) and then click on _Ok_.
![NMM searching for games](Images/NMM%20searching%20for%20games.png)
2. NMM shows then a game selection window, with a list of games which mods NMM is managing. Select _Fallout 3_ and click on _Ok_. You can select _Don't ask me next time_, if you feel like to. However, you can change the game once you start NMM.
![NMM select Fallout 3](Images/NMM%20select%20Fallout%203.png)
3. NMM needs to know the paths where the mods are going to be stored before installing them, and so it reminds you. Click on _Ok_.
![NMM setup paths](Images/NMM%20setup%20paths.png)
4. NMM has already made sensible choices for you, but feel free to change the suggested paths if you want. When you are finished, click _Finish_.
![NMM confirm paths](Images/NMM%20confirm%20paths.png)
5. NMM may organize your mods in categories, but I don't find that useful. It might be if you have a fuckload of mods, but then, I would recommend long holidays in a quiet and computer-free place, for the sake of your sanity. I would say no in the next window, but it's up to you.
![NMM no categories](Images/NMM%20no%20categories.png)
6. Finally, the programs is started, in the _Mods_ tab.
![NMM mods tab](Images/NMM%20mods%20tab.png)
7. If you take a look at the _Plugins tab_, you can check the presence of the unofficial patch, at the bottom of the load order, as expected.
![NMM plugins tab](Images/NMM%20plugins%20tab.png)
8. Open [_Fallout Stutter Remover_](http://www.nexusmods.com/fallout3/mods/8886/) mod page in your browser and navigate to the _Files_ tab. We need the latest version (4.1.36 as of this writing) and nothing else. Download this with NMM. The mod is fairly small, so it takes a breeze to download. When downloaded, you should see something like this in NMM (adjust the user interface as necessary).
![NMM FSR downloaded](Images/NMM%20FSR%20downloaded.png)
9. Double-click on the name of the FSR mod in the main panel to install it. Now, you should see a little green check mark to the left of the name of the mod, along with a message in the _Mod Activation Queue_ panel reporting that the installation is complete.
![NMM FSR installation](Images/NMM%20FSR%20installation%20complete.png)
10. Edit the file `sr_Fallout_Stutter_Remover.ini` in `[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data\FOSE\Plugins]` and change the value of the `bInject_iFPSClamp` to 1. Save the file and we are good to go!



### <a id="fakeFullScreen"></a>3.9. Fake full-screen mode

Believe or not, one of the things that could produce a CTD every other game, is the full-screen mode. As usual, Gopher has a [video explaining the problem](https://www.youtube.com/watch?v=tONiXNbwSt0) (26:38), same as before (this part spans roughly from 17:30 to the end).

1. Download manually the file _FalloutFullscreenNV_2_2_ from [_Fake Fullscreen Mode Windowed_](http://www.nexusmods.com/fallout3/mods/16001/) mod, not with NMM.
2. Extract the contents of the downloaded archive to a location of your choice.
3. Inside that folder there should be just one file, `Fallout_Fullscreen.exe`. Copy the file to `[%STEAM_HOME%\steamapps\common\Fallout 3 goty]`.
4. Create a shortcut to `Fallout_Fullscreen.exe` wherever you want, and rename it to _Fallout 3 (fullscreen)_, for example.
![Fallout 3 launch shortcuts with fullscreen](Images/Fallout%203%20launch%20shortcuts%20with%20fullscreen.png)
5. Run the launcher (_Fallout 3 (config)_, remember?), and select _Options_. Take note of your current resolution.
![Fallout 3 options](Images/Fallout%203%20options.png)
6. Mark _Windowed mode_ and change the resolution to the previous one (every time you change to windowed mode and back, the resolution combo resets). Click _Ok_ and exit the launcher.
![Fallout 3 options windowed](Images/Fallout%203%20options%20windowed.png)
7. Run the game with the new shortcut. The game will start with a window border, but after a little while, the window border disappears, resembling the actual fullscreen mode. This version is fully compatible with FOSE, which you can test running `GetFOSEVersion` in the console.



### <a id="casm"></a>3.10. Saving games the right way

The Sun rises in the East, Michael Fassbender is better than you in everything and _Fallout 3_ crashes. You need to come to terms with these simple Truths of Life.

Even with a fully patched game, _Fallout 3_ spits you out to the desktop now and then. In these cases, your only way back is to restore a saved game. But saved games do get corrupted sometimes. And, unless you have been saving your game **A FUCKING LOT**, and when I say "saving", I mean _not quicksaving_, you are doomed.

There is a mod called [CASM](http://www.nexusmods.com/fallout3/mods/3729/) to address that problem. CASM automates saving your game in a sensible way, and it provides two key shortcuts to replace the standard quicksave/quickload built-in feature:

* <kbd>F4</kbd> replaces <kbd>F5</kbd>, creating a _named_ saved game.
* <kbd>F8</kbd> replaces <kbd>F9</kbd>, loading the last saved game.

CASM also saves the game automatically with a given frequency and under certain events. Let's see how to install this mod.

1. Launch the game. When the main menu appears, click on _Settings_ and then _Gameplay_.
![Fallout 3 gameplay settings](Images/Fallout%203%20gameplay%20settings.png)
2. Disable all three options (_Save On Rest_, _Save On Wait_ and _Save On Travel_).
![Fallout 3 autosave disabled](Images/Fallout%203%20autosave%20disabled.png)
3. Press _Back_, then _Back_, then _Quit_ to exit the game.
4. Download _CASM_v1_2_3_ file from CASM using NMM.
![NMM CASM downloaded](Images/NMM%20CASM%20downloaded.png)
5. Activate CASM double-clicking on the mod name.
![NMM CASM installation complete](Images/NMM%20CASM%20installation%20complete.png)
6. Check that CASM is loaded at the bottom of the mod stack in the _Plugins_ tab of NMM.
![NMM CASM loaded last](Images/NMM%20CASM%20loaded%20last.png)
7. Close NMM and run LOOT. Click on the _Sort Plugins_ icon to fix the load order. Notice that CASM still sits at the bottom, and no conflicts are detected (this step is fairly unnecessary, but you need to get used to routinely rearrange your load order).
![LOOT after installing CASM](Images/LOOT%20after%20installing%20CASM.png)
8. This should be your load order:
	* `Fallout 3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* **`CASM.esp`**
9. CASM is configurable through an in-game option in your Pip-Boy 3000 (you will get your own Pip-Boy at the age of 10). Fire up your Pip-Boy by pressing <kbd>TAB</kbd> and navigate to the _Items_ button, _Aid_ section. You will see an "item" called _CASM Options Menu_.
![Fallout 3 CASM option](Images/Fallout%203%20CASM%20option.png)
10. Click on the CASM item _and then exit the Pip-Boy_ by pressing again <kbd>TAB</kbd> (yeah, not the most intuitive thing in the world). A screen with CASM settings is shown. There are a lot of options for you to configure, although the default settings are pretty good to go.
![Fallout 3 CASM settings](Images/Fallout%203%20CASM%20settings.png)



### <a id="adoptUselessRock"></a>3.11. Adopt an useless rock today!

_Fallout 3_ developers show their love for the details in every corner of the game.

In a slightly manic way.

The game engine is not rock solid, to begin with (no pun intended, I swear), but when it comes to handle zillions of useless objects for the sake of just showing you have zillions of rocks around you... Well, **NO**.

There is a mod which does something seemingly very simple: removing all unused objects from the game, improving performance. This mod is called [_Better Game Performance_](http://www.nexusmods.com/fallout3/mods/13520/).

Let's install this mod.

1. Download the file _V\_4_ with NMM.
![NMM Better Game Performance downloaded](Images/NMM%20Better%20Game%20Performance%20downloaded.png)
2. Activate the mod by double-clicking on its name. The mod will be installed with no hiccups.
![NMM Better Game Performance installed](Images/NMM%20Better%20Game%20Performance%20installed.png)
3. Run LOOT to rearrange your load order. The newly installed mod should sit at the bottom of your load order.
	* `Fallout 3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `CASM.esp`
	* **`BetterGamePerformance.esp`**

That's it. We have removed a lot of unused objects from the game. It's difficult to show the difference, because, these are mainly rocks, but take my word for it.




## <a id="enhancingGame"></a>4. Enhancing the game

What comes next is pretty much a matter of personal taste. While fixing the game should be completed head to toe for everyone, enhancing the game is something you need to consider, balancing pros and cons.

A rule of thumb: less is more. The fewer mods you install, the better. That said, there are a few areas where the game can be greatly improved.

Mods in this section roughly fall into one of these categories:

* Overhauls.
* Graphics enhancements.
* Audio enhancements.
* User interface enhancements.

It is tempting to install 200 mods, yelling "WOW!" each time you step into one awesome mod you suddenly discover you cannot live without. Nevertheless, before installing a new mod, think carefully, because you will need to:

* Install the mod.
* Rearrange the load order.
* Maybe install compatibility patches with other mods previously installed.
* Create and fine tune a merged patch to avoid crashes.

This is not for the faint of heart, and, remember, our goal is _to play the game_, not _to play the best fucking overmodded possible game_.

When it comes to mods, not only the load order is important, but also the [_install order_](http://www.ign.com/wikis/fallout-3/PC_Mods#Install_Order). You need to be careful, because some mods overwrite files previously written (or overwritten) by other mods.



### <a id="improvingUserInterface"></a>4.1. Improving the user interface

The first thing we are going to improve is the user interface.

Bethesda games have, broadly speaking, a shitty user interface, designed with blind, spastic monkeys in mind. The fonts are humongous, the menu layout is weird, and so forth and so on.

Thus, we are starting with a series of mods that have a low impact on the overall state of the game and, at the same time, are pleasant and noticeable.

There are several videos to warm up the engines: one to cover [the installation of the mods](https://www.youtube.com/watch?v=aqCzCXEydwU) (25:05), and the other to explain how to [stitch them all together](https://www.youtube.com/watch?v=bTlXOqV6pBA) (4:42) (there is also an [extended version](https://www.youtube.com/watch?v=qSA2BFQ2zc4) (11:23)).


#### <a id="buildingBasement"></a>4.1.1. Building the basement

First things first, we are going to need a way for all the mods to collaborate seamlessly, and for this, we are going to install [_User Interface Organizer_](http://www.nexusmods.com/fallout3/mods/20867/), or UIO. This mod will keep every important user interface mod out there in line.

If you have followed the guide so far, you have a grasp of the basics to download, activate and reorder any mod, so:

1. Download UIO with NMM.
2. Activate it.

And that's really it. No need to use LOOT because this is a FOSE plugin. FOSE plugins are placed in `[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data\FOSE\Plugins]`, so there should be a file named `ui_organizer.dll` in that folder.


#### <a id="faceWashingHUD"></a>4.1.2. Face-washing the HUD

Next, we are going to _shrink_ the user interface using [_DarNified UI F3_](http://forums.bethsoft.com/topic/1121454-wipzbeta-darnified-ui-f3/), or DUIF3.

This will be a bit tricky, because there are no NMM packages right out-of-the-box. Instead, we have the FOMOD ([_Fallout Mod Manager_](http://www.nexusmods.com/fallout3/mods/640/)) packages... But they are compatible with NMM, so bear with me.

1. Download [DUIF3 Alpha<sup>11</sup>](http://ui.darnified.net/wip/F3/dui_f3a11.zip). The file is called `dui_f3a11.zip`.
2. Download [DUIF3 Alpha<sup>11</sup> Hotfix](http://ui.darnified.net/wip/F3/dui_f3a11_HF.7z). The file is called `dui_f3a11_HF.7z`.
3. Unzip the main file (`dui_f3a11.zip`) in a location of your choice. The zipped file should contain just one file, `dui_f3a11.fomod`.
4. `.fomod` files are, in fact, `.zip` files, so you can use 7-Zip or WinRAR to unzip the file `dui_f3a11.fomod` to a location of your choice, say `[%DUIF3%]`.
5. Unzip the hotfix (`dui_f3a11_HF.7z`) and copy the contents of the unzipped file into the folder `[%DUIF3%]` we just created. Overwrite files when necessary.
6. Compress the contents of the folder `[%DUIF3%]` into a file called `darNifiedUI F3 Alpha11.zip`. The root of the file should contain the following folders, just for you to check.
	* `[Docs]`
	* `[fomod]`
	* `[menus]`
	* `[meshes]`
	* `[textures]`
7. Start NMM, go to the _Mods_ tab and click on the green plus sign to add mod from file.
![NMM Adding mod from file](Images/NMM%20Adding%20mod%20from%20file.png)
8. In the file selector that appears, navigate to the location of `darNifiedUI F3 Alpha11.zip` and choose it.
![NMM DUIF3 files loaded](Images/NMM%20DUIF3%20files%20loaded.png)
9. Activate the mod file by double-clicking on it. Eventually, you will be asked to confirm if you want to use the fonts provided with DUIF3. As crazy as it sounds, you want to say _No_, for now.
![NMM DUIF3 font config confirmation](Images/NMM%20DUIF3%20font%20config%20confirmation.png)
10. DUIF3 is finally installed.
![NMM DUIF3 installed](Images/NMM%20DUIF3%20installed.png)
11. Just in case, use LOOT to sort your load order session. It is not really necessary, as DUIF3 sits on the bottom, but you need to flex your muscles now and then.
![LOOT DUIF3](Images/LOOT%20DUIF3.png)
12. Check your load order:
	* `Fallout 3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `CASM.esp`
	* `BetterGamePerformance.esp`
	* **`DarNifiedUIF3.esp`**
13. Remember when we said "no" to use the fonts provided by DUIF3? There is an error in NMM, possibly related to modifying files in certain protected Windows folders, which crashes the program. So, go back to the [DUIF3 page](http://forums.bethsoft.com/topic/1121454-wipzbeta-darnified-ui-f3/) and copy the text block starting with `[Fonts]`. I have even done half the job for you.
```INI
[Fonts]
;sFontFile_1=Textures\Fonts\Glow_Monofonto_Large.fnt
sFontFile_1=Textures\Fonts\DarN_FranKleinBold_14.fnt
;sFontFile_2=Textures\Fonts\Monofonto_Large.fnt
sFontFile_2=Textures\Fonts\DarN_FranKleinBold_16.fnt
sFontFile_3=Textures\Fonts\Glow_Monofonto_Medium.fnt
;sFontFile_4=Textures\Fonts\Monofonto_VeryLarge02_Dialogs2.fnt
;sFontFile_4=Textures\Fonts\DarN_FranKleinBold_Otl_12.fnt
sFontFile_4=Textures\Fonts\DarN_Sui_Generis_Otl_10.fnt
sFontFile_5=Textures\Fonts\Fixedsys_Comp_uniform_width.fnt
;sFontFile_6=Textures\Fonts\Glow_Monofonto_VL_dialogs.fnt
;sFontFile_6=Textures\Fonts\DarN_PetitaMedium_Outline_18.fnt
;sFontFile_6=Textures\Fonts\DarN_Forgotten_Futurist_Otl_18.fnt
sFontFile_6=Textures\Fonts\DarN_Sui_Generis_Otl_13.fnt
;sFontFile_7=Textures\Fonts\Baked-in_Monofonto_Large.fnt
sFontFile_7=Textures\Fonts\DarN_Libel_Suit_Otl_24.fnt
;sFontFile_7=Textures\Fonts\DarN_Klill_Outline_20.fnt
sFontFile_8=Textures\Fonts\Glow_Futura_Caps_Large.fnt
```
14. Open the file `FALLOUT.INI` in `[%USERPROFILE%\Documents\My Games\Fallout3]` and paste the text over the contents of the `[Fonts]` section.
15. Launch the game and check the Vault-boy head in the lower-left corner of the screen. If you hover with the mouse over the head, you will see something like that (version numbers may vary):
```
Fallout 3 1.7.0.3
DarNified UI F3 0.11.1a
Powered by FOSE 1.2 b2
```
16. As a collateral effect, _LIVE_ button in the main screen is enabled again, but fear not! This is nothing but DUIF3 taking full control of your interface settings in a somewhat standard way. GFWL is still disabled.
![Fallout 3 DUIF3 installed](Images/Fallout%203%20DUIF3%20installed.png)
17. However, I don't like that option to be visible, so open the file `DUIF3Settings.xml` in `[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data\Menus\prefabs]` with your favorite text editor. Change the option `<_sm_hideLIVE />` to 1. Save and exit. Launch the game to check the absent LIVE option.
![Fallout 3 DUIF3 absent LIVE option](Images/Fallout%203%20DUIF3%20absent%20LIVE%20option.png)
18. Start a new game or continue a previous one, and check the smaller HUD elements, including new information about date and time in the upper-right corner of the screen.
![Fallout 3 DUIF3 small HUD](Images/Fallout%203%20DUIF3%20small%20HUD.png)
19. If you press <kbd>ESC</kbd> in game, you will see a new option at the right to configure DUIF3.
![Fallout 3 DUIF3 ingame option](Images/Fallout%203%20DUIF3%20ingame%20option.png)
20. There are a lot of settings for you to configure, adjusting the HUD to your liking.
![Fallout 3 DUIF3 settings](Images/Fallout%203%20DUIF3%20settings.png)


#### <a id="rearrangingThings"></a>4.1.3. Rearranging things

For those of you who don't like the default layout of the Heads Up Display (HUD), there is a little mod (little in size, that is) which helps you to change exactly that: [_Adjustable HUD_](http://www.nexusmods.com/fallout3/mods/15886/) or aHUD.

1. Download the mod with NMM, as usual. Take care to download the DarNified UI F3 version.
2. Activate it in the _Mods_ tab by double-clicking on its name.
3. The mod changes files installed by DUIF3, so answer _Yes to all_ when asked to overwrite files.
4. Run LOOT and sort your load order, which should be:
	* `Fallout 3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* **`aHUD.esm`**
	* `CASM.esp`
	* `BetterGamePerformance.esp`
	* `DarNifiedUIF3.esp`
5. Launch the game and press <kbd>F6</kbd> in-game to show the aHUD settings menu.
![Fallout 3 aHUD settings](Images/Fallout%203%20aHUD%20settings.png)
6. Using the menu options you can select any of the following items to relocate:
	* Compass.
	* Hitpoints.
	* Actions points.
	* Weapon condition and ammo.
7. Select the items you want to relocate and move them around using the numpad arrow keys (that is <kbd>Num8</kbd>, <kbd>Num2</kbd>, <kbd>Num4</kbd> and <kbd>Num6</kbd> for up, down, left and right, respectively). The <kbd>R</kbd> and <kbd>Num5</kbd> keys are used to reset the current movement operation (be careful; I restarted unintentionally the movement of the compass three times because I am used to the arrow keys, so I insisted on using <kbd>Num5</kbd> as "Down", instead of <kbd>Num2</kbd> `¬¬`). Any other key finishes the movement operation.
![Fallout 3 aHUD relocated items](Images/Fallout%203%20aHUD%20relocated%20items.png)

Take into account that if you plan to keep on installing mods using this guide, you may not want to relocate your HUD items, because several of the mods overwrite the XML files used to keep the HUD layout.


#### <a id="seeingThingsWhenNeeded"></a>4.1.3. Seeing things just when you need to

In addition to have the HUD elements placed where you like, you can improve the immersion by hiding these elements when you don't need them. I like to have them hidden when I am wandering around and have them shown when I am in combat. We have [_Immersive HUD_](http://www.nexusmods.com/fallout3/mods/15790/) or iHUD for this.

1. Download the mod with NMM. We are saving the file _Immersive HUD - Darnified FWE Patch_ for later, when we install _Fallout 3 Wanderer's Edition_.
2. Activate it, the usual way.
3. Answer _Yes to all_ when asked to overwrite files.
4. Use LOOT to sort your load order, which should be:
	* `Fallout 3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* **`iHUD.esm`**
	* `CASM.esp`
	* `BetterGamePerformance.esp`
	* `DarNifiedUIF3.esp`
5. Launch the game and notice the absence of HUD elements on screen.
![Fallout 3 iHUD default](Images/Fallout%203%20iHUD%20default.png)
6. Keep the <kbd>I</kbd> key pressed a few moments. The iHUD settings menu will appear.
![Fallout 3 iHUD settings](Images/Fallout%203%20iHUD%20settings.png)
7. There are a lot of customization options in iHUD. Tweak around until you feel comfortable with the results ([Gopher's video](https://youtu.be/aqCzCXEydwU?t=18m20s) should help, around 18:20).

A final step: we are going to create a backup copy of the folder with the menu definitions (`[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data\Menus]`).

Why this backup? Well, there are a lot of mods which change the user interface, and we are going to use them. In these matters, installation order is more important than load order, because each mod _overwrites_ several files to fulfill its own goals, thus losing the modifications created by previous mods.

The way we are installing mods in this guide is more functional than technical, so the installation order we are following is less than ideal. However, we are going to manually keep track of the changes made by each mod to stitch all them together.


#### <a id="retexturingPipBoy"></a>4.1.4. Cleaning up your faithful companion

One of the things you are going to see a lot in this game is your Pip-Boy. And when I say "a lot", I mean an awful-fucking lot. It's your personal assistant, after all.

It's a little sad to see that glorious piece of junk in low resolution, so, let's improve how it looks, using:

* [_PipBoy 3000 HD Retexture_](http://www.nexusmods.com/fallout3/mods/20373/)
* [_Shiloh DS - Clean Pipboy Screen_](http://www.nexusmods.com/newvegas/mods/36255/) (this is a _Fallout New Vegas_ mod, but it works anyway).
* [_Faster Pipboy Faster_](http://www.nexusmods.com/newvegas/mods/35225/) (same as before).

1. Download _PipBoy 3000 HD Retexture - PC and Xbox Controller Versions_ with NMM.
2. Download _Faster Pipboy Faster_ manually. NMM detects this mod is not specifically designed for _Fallout 3_, so it cannot download the file.
3. Download _Shiloh DS - Clean Pipboy Screen v1\_4_ manually (same reasons as before).
4. Add the two _Fallout New Vegas_ mods to NMM using the button _Add mod from file_. We will have all the files ready in NMM by then.
![NMM cleaning Pip-Boy mods](Images/NMM%20cleaning%20Pip-Boy%20mods.png)
5. Activate _PipBoy 3000 HD Retexture - PipBoy 3000 HD Retexture - PC and Xbox Controller Versions_ first. There shouldn't be any overwriting.
6. Activate _Faster Pipboy Faster-35225_ next. No conflicts should arise, either.
7. Finally, activate _Shiloh DS - Clean Pipboy Screen_. A window with several options will appear. We will choose:
	* Remove Scanlines.
	* Remove Screen Glare.
	* Remove Distorting Effects.
	* Add Pure Black BG.
	* Remove Map Tinting.
	* Glow Intensity 128% (default).
	* Standard compatibility.
![NMM Clean Pip-Boy options](Images/NMM%20Clean%20Pip-Boy%20options.png)
8. The mod overwrites several files installed by DUIF3, so answer _Yes to all_ when asked to.
9. Launch the game and pull out your Pip-Boy with the <kbd>TAB</kbd> key. You will notice a piece of junk hitting your face at full speed, and also a dramatic change in the cleanliness of the screen. Compare before and after.
![Fallout 3 Pip-Boy before retexturing](Images/Fallout%203%20Pip-Boy%20before%20retexturing.png)
![Fallout 3 Pip-Boy after retexturing](Images/Fallout%203%20Pip-Boy%20after%20retexturing.png)


#### <a id="betterMap"></a>4.1.5. You don't want to ask for directions

Let's face it: the vanilla map in _Fallout 3_ seems to have been produced from Dora the Explorer's backpack. And you don't want to start asking directions in D.C., because super-mutants are not known for their kindness of heart with strangers.

We are going to use [_Better High Detail Map and Icons_](http://www.nexusmods.com/fallout3/mods/16898/) to have decent maps, along with [_No more dots_](http://www.nexusmods.com/fallout3/mods/15918/) to get rid of the white dotted line that tells you the shortest path between you and a suitable [Darwin Awards](http://www.darwinawards.com/) death, because in mathematics the straight line may be the shortest path between two points, but in real life, and specially in the Capital Wasteland, it's a ticket to Hell.

1. Download _Better High Detail Map and Icons_ with NMM. It will take a while, because the texture files are pretty big (43 MB or so).
2. Download _no more dots v01_ with NMM.
2. Activate NMM shows a floating window with the installation options for the mod. Choose one map size and brightness (I chose 8k with roads and 50% more brightness, but your mileage may vary). Click on _Next_.
![NMM Better High Detail Map and Icons install options](Images/NMM%20Better%20High%20Detail%20Map%20and%20Icons%20install%20options.png)
3. Next window contains the customization options for the mod. I checked "Custom icons" and green markers. It is important **not to check** "Clean Pipboy Screen", because we applied a specific mod to do just that in the previous chapter. Click on _Finish_.
![NMM Better High Detail Map and Icons customization options](Images/NMM%20Better%20High%20Detail%20Map%20and%20Icons%20customization%20options.png)
4. Answer _No to all_ when asked to overwrite files. The mod tries to overwrite files from _Shiloh DS - Clean Pipboy Screen_, but the files are just fine.
5. Activate _no more dots - no more dots  v01_. No overwriting required.
5. Launch the game, fire up your Pip-Boy and compare, before and after.
![Fallout 3 world map before](Images/Fallout%203%20world%20map%20before.png)
![Fallout 3 world map after](Images/Fallout%203%20world%20map%20after.png)


#### <a id="shedSomeLight"></a>4.1.7. Shed some light here, please

Lighting in _Fallout 3_ is somewhat weird. Sometimes you will find your self into what seems to be a lucid LSD-induced dream, with overexposed lights all around you. If you use your Pip-Boy's lamplight, things get much worse.

This small mod, [_SmoothLight - Pip-Boy Light Enhancer_](http://www.nexusmods.com/fallout3/mods/18389/), comes to the rescue. Here we go.

1. Download and activate the mod with NMM. There shouldn't be any conflicts.
2. Use LOOT to sort your load order, which should be:
	* `Fallout 3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CASM.esp`
	* `BetterGamePerformance.esp`
	* `DarNifiedUIF3.esp`
	* **`HZSmoothLight - FO3.esp`**
3. Launch the game and activate your Pip-Boy's lamplight long-pressing the <kbd>TAB</kbd> key in a dark area.

See the difference for yourself.

With no light:

![Fallout 3 no Pip-Boy light](Images/Fallout%203%20no%20Pip-Boy%20light.png)

With standard light:

![Fallout 3 standard light](Images/Fallout%203%20standard%20light.png)

With enhanced light:

![Fallout 3 enhanced light](Images/Fallout%203%20enhanced%20light.png)

The difference is subtle, more noticeable in dark interiors.



### <a id="lendMeYourEars"></a>4.2. Lend me your ears

Audio is one of the most underrated aspects in videogames. There is an unfortunate term coined for those gamers craving for the ultimate graphics experience: _graphic whores_. For audio? There is none, except if you would consider _audiophile_, but that has not the same taste.

Gaming experience is built on top of both graphics and audio. The latter is a subtle part, but very important, nonetheless. Good ambient sounds and soundtrack can make your journey something memorable.

In this chapter we will take care of that, changing the way you hear and listen to the Wasteland.


#### <a id="hearingNukesFly"></a>4.2.1. Hearing the nukes fly in high quality

There is just one mod in this chapter, [_Fallout 3 - HD Audio Overhaul - v1.21_](http://www.nexusmods.com/fallout3/mods/13055/), and it's a complete overhaul of all things related with audio in _Fallout 3_, from ambient sounds to soundtrack.

This mod is _massive_, so grab a mug of coffee and stay tuned with the latest news while installing it. You just have to download and install it with NMM. No conflicts should arise. No need to rearrange the load order, either, for there is not `.esp` or `.esm` installed.

Launch the game and _listen_ carefully...


#### <a id="thoseCrickets"></a>4.2.2. Those crickets are driving me mad

Imagine yourself wandering at night in the radioactive wastes of the slums in D.C. There are a lot of things going on, even in a desolate barren like this: insects, night birds of prey, dogs, etc. These are the small things that boost a real sense of immersion in the game.

[_Ambient Wasteland 2_](http://www.nexusmods.com/fallout3/mods/12602/) is for ambient sounds what [_Fallout 3 HQ Audio Overhaul_](http://www.nexusmods.com/fallout3/mods/13055/) is for music. It changes the small sounds of the Wasteland so you can shit your pants looking for that owl you heard in the dark.

1. Download _Ambient Wasteland 2 WAV edition_ with NMM. Be careful: we want the WAV edition, not the MP3 edition. We want to give it all we've got.
2. Download _Ambient Wasteland 2 Wav Patch_ with NMM.
3. Activate them in the same order you downloaded them. The patch will overwrite files from the main file. Otherwise, there will be no conflicts.

And that's really it. Launch the game and search for a deserted area with no imminent danger. Sit back and listen.


#### <a id="radioStations"></a>4.2.3. A soundtrack for your lonely Wasteland nights

I have to confess I have never listened to a single radio station in the game in any of my playthroughs. I usually prefer to listen to the ambient sounds, because you'll never when you are about to become the next meal of a hungry deformed creature.

Radio stations, not being my cup of tea (with butter, Tibet style), are an immersive piece of lore, though. We are going to add two new radio stations and to improve an existent one:

* [_GNR Enhanced_](http://www.nexusmods.com/fallout3/mods/14946/): 100 additional songs to the 20 original in _Galaxy News Radio_.
* [_CONELRAD 640-1240 - Civil Defense Radio_](http://www.nexusmods.com/fallout3/mods/6104/): A new station with _real_ Civil Defense broadcasting messages.
* [_Existence 2_0 - Robot Radio_](http://www.nexusmods.com/fallout3/mods/5612/): Can you imagine a robot with existential dread? Well, that's what you get with this radio station.

Let's go, then.

1. Download _GNR Enhanced_ with NMM. Download _Beta Update_ too. The main file is _huge_, so go and get a Nuka-Cola somewhere.
2. Download _Conelrad 640-1240_ with NMM.
3. Download _Existence 2.0_ with NMM.
4. Activate them in any order. There will be no overlapping, except for the _Beta Update_ in GNR.
5. Run LOOT to rearrange your load order:
	* `Fallout 3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CASM.esp`
	* `BetterGamePerformance.esp`
	* `DarNifiedUIF3.esp`
	* `HZSmoothLight - FO3.esp`
	* **`GNR Enhanced.esp`**
	* **`Existence 2.0.esp`**
	* **`Conelrad 640-1240.esp`**

You will need to be in the station's range to tune in (_Data_ button, _Radio_ section in your Pip-Boy), but when you do, enjoy the rhythm! _Conelrad 640-1240_ and _Existence 2.0_ will be immediately available right after leaving Vault 101.

![Fallout 3 new radio stations](Images/Fallout%203%20new%20radio%20stations.png)



### <a id="playingBadAss"></a>4.3. Playing the bad-ass way

We have a pretty much vanilla game up to this point. Yeah, we changed the way the game looks and sounds in the previous chapter, but the base game still remains the same.

We are going to dramatically change that. Think of a chicken nugget that turns itself into a _filet mignon_, all of a sudden.


#### <a id="adAstraPerAspera"></a>4.3.1. _Ad astra per aspera_

The title of this chapter means "through hardships to the stars", in Latin, and it would be a good way to define our next mod: [_Fallout 3 Wanderers Edition_](http://www.nexusmods.com/fallout3/mods/2761/), or FWE. Xuul has a video [explaining how to install FWE](https://www.youtube.com/watch?v=J4y4lui3l9U) (15:16), and there is a [page for the project](https://sites.google.com/site/fo3wanderersedition) with lots of useful information.

The list of changes made by FWE is so long and their implications so deep that you'd better read the mod page to get a glimpse of that. The bottom line is: you will be playing a harsher, more challenging version of the game.

We will be needing five files:

* _FWE Master Release 6-0 - Part 1._
* _FWE Master Release 6-0 - Part 2._
* _FWE 6-03a HOTFIX PATCH._
* _DarnUI Support for FWE 6-02_
* _Immersive HUD - iHUD - Immersive HUD - Darnified FWE Patch_

The last one can be downloaded from [the iHUD page](http://www.nexusmods.com/fallout3/mods/15790/).

1. Download the three FWE files _manually_, not with NMM, in a location of your choice.
2. Download the two remaining files with NMM, but _do not activate them_.
3. Create a folder in a location of your choice, say `[%FWE_FULL%]`.
4. Unzip the file `FWE Master Release 6-0 - Part 1-2761.7z` in a location of your choice (say `[%FWE_PART_1%]`), using [7-Zip](http://www.7-zip.org/), for example.
5. Unzip the file `FWE Master Release 6-0 - Part 2-2761.7z` in a location of your choice (say `[%FWE_PART_2%]`).
6. Unzip the file `FWE 6-03a HOTFIX PATCH-2761.7z` in a location of your choice (say `[%FWE_HOTFIX%]`).
7. Copy the contents of the folder `[%FWE_PART_1%]` into the folder `[%FWE_FULL%]`.
8. Copy the contents of the folder `[%FWE_PART_2%]` (except the folder `[fomod]`) into the folder `[%FWE_FULL%]`, overwriting when necessary.
9. Copy the contents of the folder `[%FWE_HOTFIX%]` (except the folder `[fomod]`) into the folder `[%FWE_FULL%]`, overwriting when necessary.
10. Create a ZIP file (say `FWE_6.03.zip`) with _the contents of the folder_ `[%FWE_FULL%]`. The compression will take a while, for the mod contents weight over 1 GB. The root of the zipped file should have the following folders, just to check:
	* `[fomod]`
	* `[Meshes]`
	* `[Sound]`
	* `[Textures]`
11. Add `FWE_6.03.zip` to NMM, like we did before with DarNifiedUI.
![NMM FWE add mod from file](Images/NMM%20FWE%20add%20mod%20from%20file.png)
12. We have all the files ready to install.
![NMM FWE entries](Images/NMM%20FWE%20entries.png)
13. Double click on _FWE - FO3 Wanderers Edition_ to bring up a window with some options. Leave all default options checked and check _Alternate Travel_, and maybe [_VATS Halftime_ and _VATS Realtime_](https://sites.google.com/site/fo3wanderersedition/detailed-changes/02combat#TOC-VATS-Tweaks) if you feel up to.
![NMM FWE setup](Images/NMM%20FWE%20setup.png)
14. The installation takes a while, for the mod is _huge_...
![NMM FWE installing](Images/NMM%20FWE%20installing.png)
15. Finally, the manager notifies us about a successful installation. There shouldn't be any conflicts.
![NMM FWE installed](Images/NMM%20FWE%20installed.png)
16. Double click on _FWE - FO3 Wanderers Edition - DarnUI Support for FWE 6-02_ and answer _Yes to all_ when asked to overwrite files.
17. Double click on _Immersive HUD - iHUD - Immersive HUD - Darnified FWE Patch_ and answer _Yes to all_ when asked to overwrite files.
18. Due to the install order we are following (functional, instead of technical), the two user interface patches we have just activated make a little mess of the HUD. To correct that, I have created a small patch of my own (_Modding never changes DUIF3-FWE patch_) with the merged files. Download the patch, add it to NMM and activate it, overwriting files when needed.
19. A number of files has been installed, so we need to rearrange our load order. Fire up LOOT and sort the files. This should be your load order:
	* `Fallout 3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* **`CRAFT.esm`**
	* **`CALIBR.esm`**
	* **`FO3 Wanderers Edition - Main File.esm`**
	* **`FO3 Wanderers Edition - Alternate Travel.esp`**
	* `CASM.esp`
	* `BetterGamePerformance.esp`
	* `GNR Enhanced.esp`
	* **`FO3 Wanderers Edition - Main File.esp`**
	* `HZSmoothLight - FO3.esp`
	* `Existence 2.0.esp`
	* `Conelrad 640-1240.esp`
	* **`FO3 Wanderers Edition - DLC Broken Steel.esp`**
	* **`FO3 Wanderers Edition - DLC Anchorage.esp`**
	* **`FO3 Wanderers Edition - DLC Point Lookout.esp`**
	* **`FO3 Wanderers Edition - DLC The Pitt.esp`**
	* **`FO3 Wanderers Edition - DLC Mothership Zeta.esp`**
	* `DarNifiedUIF3.esp`
20. LOOT warns you that certain files are somewhat dirty, so a cleaning with FO3Edit is in order. Just clean the files following the same steps we did in [the chapter about cleaning up the master files](#cleaningMasterFiles). To clean each file, select just this file in FO3Edit and let the tool select the set of files it depends on. For example, if you select `FO3 Wanderers Edition - Main File.esm`, the following files will be loaded altogether:
	* `Fallout3.esm`
	* `Fallout3.exe`
	* `CRAFT.esm`
	* `CALIBR.esm`
21. When all the files have been cleaned, run LOOT again and check there are no ITM records or undeleted references in your load order. There shouldn't be any.
22. And that's it. We have FWE completely installed. Launch the game and start a new game (yes, a new game). At certain point, you may choose between the classic storyline or an alternate start.
![Fallout 3 FWE alternate start](Images/Fallout%203%20FWE%20alternate%20start.png)
23. You can assign your skills, perks and even a background story in a terminal right in front of you right after waking up.
![Fallout 3 FWE special terminal](Images/Fallout%203%20FWE%20special%20terminal.png)
24. When you have selected the skill set for your journey, just sleep in the mat on the floor and wake up to your new life. After a moment, a dialog will appear talking about _Wasteland Explorer_, a motorcycle which replaces fast travel (we disabled it, remember?). Enable it for good.
![Fallout 3 FWE Wasteland Explorer enabled](Images/Fallout%203%20FWE%20Wasteland%20Explorer%20enabled.png)
25. And now we are at it... Remember when we relocated the HUD elements to fit our needs? Well, FWE resets that, so, regrettably, you will have to relocate them again. Notice the new grenade icon on the right lower corner and the primary needs info under the clock.
![Fallout 3 FWE HUD reset](Images/Fallout%203%20FWE%20HUD%20reset.png)
26. Pull out your Pip-Boy and go to the _Items_ and then _Apparel_. There it is the option to configure FWE.
![Fallout 3 FWE Pip-Boy option](Images/Fallout%203%20FWE%20Pip-Boy%20option.png)
27. Click on the option to show the shitload of configurable settings for this mod.
![Fallout 3 FWE settings](Images/Fallout%203%20FWE%20settings.png)

You may be wondering why the hell we installed aHUD first and then FWE... Well, it's a matter of scalability. Each chapter in the enhancing section will give you a playable milestone. The first one was about having an improved UI, and this one is about playing a radically different game. Each section builds on top of the previous one, but, in this case, the drawbacks are no big deal.

From this point on, we will be using [_The Mergers_](http://www.nexusmods.com/fallout3/mods/16787/), from Paradox Ignition. These are merged patches for the main mods we are going to install. They are aimed to reduce the file load in our data folder and increase stability.


#### <a id="checkhovsGun"></a>4.3.2. A sound for Chekhov's gun

I have never fired a real weapon in my life, so I couldn't tell the sound of a real gun from a virtual one. However, with the [_Improved Sound FX v1\_3_](http://www.nexusmods.com/fallout3/mods/627/) mod, it's not difficult to guess which version sound better.

See, or I should say, listen for yourself, in this [lengthy video](https://www.youtube.com/watch?v=aMm31gnXzk8) (6:38) (for what it is), showcasing the difference between vanilla and improved weapon sounds. You will have a much more satisfying rain of bullets in your everyday shoot-outs.

1. Download and activate _Improved Sounds FX v13_.
2. The sound files collide with previous files installed by FWE, so answer _Yes to all_ when asked to overwrite.

By the way, this chapter should have been included into the chapter about [music and sound](#lendMeYourEars), but FWE collides with _Improved Sound FX v1\_3_ and doesn't get well along with it, so I decided to alter the functional order I have been following so far to ensure a flawless setup.


#### <a id="fraternizingNeighborhood"></a> 4.3.3. Fraternizing with the neighborhood

If you like real challenges, you will **love** [_Martigen's Mutant Mod_](http://www.nexusmods.com/fallout3/mods/3211/), or MMM, for short. MMM adds a lot of color to the game, in the form of new (and tougher) enemies, increased spawn rates, and so on.You will have plenty of rotten flesh-shaped love.

1. Download the file _Marts Mutant Mod 1-RC61 FOMOD Ready_ with NMM (yeah, half of this book is plagued with acronyms; I am acutely aware of that). No need to download the update because the merged patch we are going to use overwrites the files in it.
2. Download _Marts Mutant Mod Merged_ from [_The Mergers_](http://www.nexusmods.com/fallout3/mods/16787/) page with NMM. Notice the downloaded files.
![NMM MMM files downloaded](Images/NMM%20MMM%20files%20downloaded.png)
3. Activate _Martigen's Mutant Mod_ by double-clicking on it. NMM shows a window to select the preferred configuration method. We will choose the in-game menu, as it requires far less tinkering than its ESP counterpart.
![NMM MMM menu configuration](Images/NMM%20MMM%20menu%20configuration.png)
4. In the next window, all the DLC options should be checked, but leave the global options unchecked. More on that later.
![NMM MMM global options](Images/NMM%20MMM%20global%20options.png)
5. MMM overwrites several files from FWE, as it overhauls the monster system in the game. Let it do its magic.
![NMM MMM FWE overwrite](Images/NMM%20MMM%20FWE%20overwrite.png)
6. We are going to get rid of the files installed by MMM to use the merged path we downloaded before. Create a folder in your data folder (namely `[MMM backup]`), and move the following files:
	* `Mart's Mutant Mod.esm`
	* `Mart's Mutant Mod.esp`
	* `Mart's Mutant Mod - DLC Anchorage.esp`
	* `Mart's Mutant Mod - DLC The Pitt.esp`
	* `Mart's Mutant Mod - DLC Broken Steel.esp`
	* `Mart's Mutant Mod - DLC Point Lookout.esp`
	* `Mart's Mutant Mod - DLC Zeta.esp`
	* `Mart's Mutant Mod - Master Menu Module.esp`
7. Reopen NMM and activate _Paradox Ignition presents The Mergers - Marts Mutant Mod Merged_ in the _Mods_ tab. The merged patch will ask for permission to overwrite already installed files. Proceed as usual.
![NMM MMM merged patch overwriting](Images/NMM%20MMM%20merged%20patch%20overwriting.png)
8. There are three files installed we are not going to need, corresponding to the options we didn't choose before regarding MMM configuration. They are in the data folder (`[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data]`), and can be safely removed, because the options they provide are yet included in FWE. Navigate to the data folder and delete them.
	* `Mart's Mutant Mod - Natural Selection.esp`
	* `Mart's Mutant Mod - Tougher Traders.esp`
	* `Mart's Mutant Mod - Zones Respawn.esp`
9. In the _Plugins_ tab, check the presence of the file `Mart's Mutant Mod.esm`, replacing all the files we installed before.
![NMM MMM installed](Images/NMM%20MMM%20installed.png)
10. Run LOOT as usual and rearrange your load order. This should be the deal:
	* `Fallout 3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CRAFT.esm`
	* `CALIBR.esm`
	* `FO3 Wanderers Edition - Main File.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* **`Mart's Mutant Mod.esm`**
	* `CASM.esp`
	* `BetterGamePerformance.esp`
	* `GNR Enhanced.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* `Existence 2.0.esp`
	* `Conelrad 640-1240.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `DarNifiedUIF3.esp`
11. Launch the game and pull up your Pip-Boy. Navigate to the _Items_ button, _Apparel_ section, where you will see a new entry called _MMM Control Panel_.
![Fallout 3 MMM control panel option](Images/Fallout%203%20MMM%20control%20panel%20option.png)
12. Click on the aforementioned option and wade through the zillions of options to fine-tune your monster-hunting experience.
![Fallout 3 MMM settings](Images/Fallout%203%20MMM%20settings.png)

Take into account that we need a [_Blackened_ compatibility patch](http://www.nexusmods.com/fallout3/mods/18173/) to run FWE and MMM seamlessly, but Blackened patches come in combos (for example, FWE + MMM + EVE), so we are going to postpone the installation of a patch until we have some other mods installed.


#### <a id="weNeedMoreFirepower"></a>4.3.4. We need more firepower!

The vanilla version of _Fallout 3_ is somewhat limited regarding weapons. We'll have plenty of firepower, but the weapon effects are dull, and the customization options are basically zero. Moreover, if you are used to traditional FPSs, you will surely find the aiming system a fucking crap.

We are getting serious here, because, at the end of the chapter, we will have a completely revamped weapon system in the game. As usual, Gopher has a fantastic video [covering weapon mods](https://www.youtube.com/watch?v=Vli2y7ZDUbo) (15:02), although not all of them. I have used also a similar Xuul's [video to update the weapon systems](https://www.youtube.com/watch?v=TOSIL9k9dKk) to get cutting edge modding procedure.

We are going to install [_Weapon Mod Kits_](http://www.nexusmods.com/fallout3/mods/3388/) (WMK), [_Energy Visuals Enhanced_](http://www.nexusmods.com/fallout3/mods/8340/) (EVE) and [_Rogue Hallow's Ironsights_](http://www.nexusmods.com/fallout3/mods/6938/) (RH_IronSights), along with the corresponding [Paradox Ignition merged patches](http://www.nexusmods.com/fallout3/mods/16787/).

1. Download the following WMK files manually, not with NMM:
	* [_Weapon Mod Kits_](http://www.nexusmods.com/fallout3/download/64569)
	* [_WMK Broken Steel Compatibility Patch_](http://www.nexusmods.com/fallout3/download/62400)
	* [_WMK Mothership Zeta Compatibility Patch_](http://www.nexusmods.com/fallout3/download/64570)
	* [_WMK Operation Anchorage Compatibility Patch_](http://www.nexusmods.com/fallout3/download/53514)
	* [_WMK Point Lookout Compatibility Patch_](http://www.nexusmods.com/fallout3/download/63656)
	* [_WMK The Pitt Compatibility Patch_](http://www.nexusmods.com/fallout3/download/58184)
2. Create a folder in a location of your choice, namely `[%WMK_FULL%]`.
3. Unpack the contents of every WMK file we have downloaded into that folder. There shouldn't be any overwriting.
4. Zip _the contents_ of `[%WMK_FULL%]` into a file named `WMK.zip`. The root of this file should contain a bunch of `.esp` files, a bunch of `*_readme.txt` files and several folders.
5. Add `WMK.zip` to NMM (_Add mod from file_, in the green plus sign on the toolbar).
6. Download the following RH_IronSights files manually, not with NMM:
	* [_RH\_IronSights BETA_](http://www.nexusmods.com/fallout3/download/83555)
	* [_RH\_IronSights BETA Update 1_](http://www.nexusmods.com/fallout3/download/86279)
	* [_New Weapons for BETA_](http://www.nexusmods.com/fallout3/download/83777)
	* [_RH\_IronSights - Better Uniques_](http://www.nexusmods.com/fallout3/download/86278)
7. Create a folder in a location of your choice, say `[%RH_IRONSIGHTS_FULL%]`.
8. Unpack the contents of every RH_IronSights file we have downloaded into that folder. Overwrite files when necessary.
9. Every RH_IronSights file contained a `[Data]` folder, but we are going to simplify things a little. _Move_ all the contents of `[%RH_IRONSIGHTS_FULL%\Data]` to `[%RH_IRONSIGHTS_FULL%]` (up a level), and delete `[%RH_IRONSIGHTS_FULL%\Data]` folder.
10. Download [_RH\_Ironsights Merged_](http://www.nexusmods.com/fallout3/download/1000005036) manually from [_Paradox Ignition the Mergers_](http://www.nexusmods.com/fallout3/mods/16787/) page. This is a merged patch that allows us to reduce the number of loaded files for RH_IronSights.
11. Unpack the contents of the merged patch into `[%RH_IRONSIGHTS_FULL%]`, overwriting when necessary. Notice there is no `[Data]` folder this time.
12. Delete the following files, which are replaced by the merged patch (every `.esp` file, in fact):
	* `RH_IronSights_Basic_AnchoragePlugin.esp`
	* `RH_IronSights_Basic_BrokenSteelPlugin.esp`
	* `RH_IronSights_Basic_PittPlugin.esp`
	* `RH_IronSights_Basic_PointLookoutPlugin.esp`
	* `RH_IronSights_Basic_VanillaPlugin.esp`
	* `RH_IronSights_Basic_ZetaPlugin.esp`
	* `RH_IronSights_Pitt_NewRifleSights.esp`
	* `RH_IronSights_PL_NewItems.esp`
	* `RH_IronSights_RemoveReticule.esp`
	* `RH_IronSights_Vanilla_BetterUniques.esp`
	* `RH_IronSights_Vanilla_NewWeapons.esp`
13. Zip the contents of `[%RH_IRONSIGHTS_FULL%]` into a file named `RH_IronSights.zip`.
14. Add `RH_IronSights.zip` to NMM (_Add mod from file_, in the green plus sign on the toolbar).
15. Download _EVE 099_ file from [EVE](http://www.nexusmods.com/fallout3/mods/8340/) with NMM. Ignore the optional files.
16. Download _RH IronSights - FWE Bridge_ from [_RH\_IronSights_](http://www.nexusmods.com/fallout3/mods/6938/) with NMM.
17. Download _RH\_IronSights - EVE Bridge_ from [_RH\_IronSights_](http://www.nexusmods.com/fallout3/mods/6938/) with NMM.
18. Download _RH\_IronSights - WMK Bridge_ from [_RH\_IronSights_](http://www.nexusmods.com/fallout3/mods/6938/) with NMM.
19. We have a good bunch of mods ready to be installed.
![!NMM weapon mods ready](Images/NMM%20weapon%20mods%20ready.png)
20. Activate _WMK_ and answer _Yes to all_ when asked for overwriting files (all from the previous FWE installation).
21. Activate _EVE - Energy Visuals Enhanced - EVE 099_. Again, it's going to overwrite several FWE files.
22. Activate _RH\_IronSights_. Answer _Yes to all_ when asked to overwrite files, as usual.
23. Activate the RH_IronSights bridges, in the following order:
	* _RH\_IronSights - FOSE - RH\_IronSights - EVE Bridge_
	* _RH\_IronSights - FOSE - RH\_IronSights - WMK Bridge_
	* _RH\_IronSights - FOSE - RH IronSights - FWE Bridge_
24. We are going to need a compatibility patch to stitch all these mods together, so navigate to the [_Blackened_ compatibility patches](http://www.nexusmods.com/fallout3/mods/18173/) page, download and activated _Blackened FWE - MMM - EVE_ file with NMM.
25. Run LOOT to rearrange your load order. This should be your setup by now.
	* `Fallout3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CRAFT.esm`
	* `CALIBR.esm`
	* `FO3 Wanderers Edition - Main File.esm`
	* `Mart's Mutant Mod.esm`
	* **`EVE.esm`**
	* **`RH_IRONSIGHTS.esm`**
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `CASM.esp`
	* `BetterGamePerformance.esp`
	* `GNR Enhanced.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* `Existence 2.0.esp`
	* `Conelrad 640-1240.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `DarNifiedUIF3.esp`
	* **`Blackened FWE + MMM + EVE.esp`**
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* **`RH_FWE_Bridge.esp`**
	* **`WeaponModKits.esp`**
	* **`WeaponModKits - BrokenSteel.esp`**
	* **`WeaponModKits - OperationAnchorage.esp`**
	* **`WeaponModKits - ThePitt.esp`**
	* **`WeaponModKits - Zeta.esp`**
	* **`WeaponModKits - PointLookout.esp`**
	* **`RH_EVE_Bridge.esp`**
	* **`RH_WMK_Bridge.esp`**
26. According to LOOT, the files `RH_IRONSIGHTS.esm` and `RH_EVE_Bridge.esp` are dirty, so proceed to clean them up with FO3Edit. Remember: select just that file and the files it depends on will be automatically loaded.
27. Run the game and you will notice the dramatic change when aiming your weapon. **NOW**, this is serious shit.
![Fallout 3 new sights](Images/Fallout%203%20new%20sights.png)



### <a id="expandingYourWorld"></a>4.4. Expanding your world

This section is about adding new content to the game, and it's the last block before changing the way the game looks. We are going to add a few new places and quests, a new playable set (armor, range finder, trap detector and nightvision gear), and pulling out a feature the game actually has, but does not show by default.


#### <a id="hicSuntDracones"></a>4.4.1. _Hic sunt dracones_

It's not that _Fallout 3 Game of the Year Edition_ lacks places to visit. On the contrary, you will be ruining your life trying to unfold the secrets of the Capital Wasteland, but, still, why not add some spice to the mix?

We are going to install several mods that add new content to the game:

* [_A Note Easily Missed_](http://www.nexusmods.com/fallout3/mods/4730/)
* [_Alton, IL_](http://www.nexusmods.com/fallout3/mods/16949/)
* [_An Evening With Mister Manchester_](http://www.nexusmods.com/fallout3/mods/5630/)
* [_Arefu Expanded_](http://www.nexusmods.com/fallout3/mods/8976/)
* [_Mothership Zeta Crew_](http://www.nexusmods.com/fallout3/mods/8747/).
* [_The Institute - a fully voiced quest mod_](http://www.nexusmods.com/fallout3/mods/14449/)
* [_To sleep - perchance to dream_](http://www.nexusmods.com/fallout3/mods/6921/)
* [_Vault 101 Revisited_](http://www.nexusmods.com/fallout3/mods/13308/)

Visit each mod's page to find out more about what you will find with the new quests and areas.

Let's start.

1. Download the following files for each mod, all with NMM, unless otherwise specified:
	* _A Note Easily Missed v107_ for _A Note Easily Missed_.
	* _Alton IL Version 2-0-1_ and _Alton IL Hotfix 2-0-3_ for _Alton, IL_.
	* Manually download [_Alton Re-voiced update without lip files_](http://www.nexusmods.com/fallout3/download/1000007113) from [_Alton Revoicing Project_](http://www.nexusmods.com/fallout3/mods/20859/).
	* _Alton\_IL\_lip\_for\_Revoiced_ from [_Alton Revoiced lip files_](http://www.nexusmods.com/fallout3/mods/22041/).
	* _An Evening with Mister Manchester v181_ and _An Evening With Mister manchester v181 UPDATE_ for _An Evening with Mister Manchester_.
	* _Arefu Expanded v1\_7a - Data Files_ and _Arefu Expanded v1\_7d - ESP and ESM files_ for _Arefu Expanded_.
	* _Mothership Zeta Crew V 166 ZIP_ for _Mothership Zeta Crew_.
	* _The Institute - a fully voiced quest mod 1\_0\_1_ and _The Institute 1\_0\_1 ESM only_ from _The Institute - a fully voiced quest mod_.
	* _To sleep - perchance to dream v106_ and _To sleep - perchance to dream v1061_ for _To sleep - perchance to dream_.
	* _Vault 101 Revisited - Main 104_ for _Vault 101 Revisited_.
2. Manually add the file `Alton Re-voiced update without lip files-20859-v1-3.zip` to NMM (this is the only file not downloaded with NMM in this series).
3. Check all the files are downloaded and ready in NMM. Take into account that _Mothership Zeta Crew_ is **HUGE** (over 1 GB), so be patient and make the most of your time reading online documentation about creating a book using Asciidoc, for example.
![NMM new content mods](Images/NMM%20new%20content%20mods.png)
4. We are going to activate _Alton, IL_ files first, because there is a main file and several patches. Activate them in the following order, overwriting when asked to.
	* _Alton IL - Huge World and Quest Mod - Alton IL Version 2-0-1_
	* _Alton IL Hotfix 2-0-3 RC_
	* _Alton Revoicing Project_
	* _Alton Revoiced lip files - Alton\_IL\_lip\_for\_Revoiced_
5. Activate the following files next, in this order, overwriting original files with patches/updates:
	* _Arefu Expanded v1\_7d by Azar - Arefu Expanded v1\_7a - Data Files_
	* _Arefu Expanded v1\_7d by Azar - Arefu Expanded v1\_7d - ESP and ESM files_
	* _Mothership Zeta Crew - Mothership Zeta Crew V 166 ZIP_
	* _A Note Easily Missed - A Note Easily Missed v107_
	* _An Evening With Mister Manchester - An Evening with Mister Manchester v181_
	* _An Evening With Mister Manchester - An Evening With Mister manchester v181 UPDATE_
	* _The Institute - a fully voiced quest mod - The Institute - a fully voiced quest mod 1\_0\_1_
	* _The Institute - a fully voiced quest mod - The Institute 1\_0\_1 ESM only_
	* _To sleep - perchance to dream - To sleep - perchance to dream v106_
	* _To sleep - perchance to dream - To sleep - perchance to dream v1061_
	* _Vault 101 Revisited - Vault 101 Revisited - Main 104_
6. When all them mods are installed, fire up LOOT to rearrange your load order. Ignore the load order for now, because there are several dirty files we have to clean first. These are the dirty files to clean with FO3Edit:
	* `Vault 101 Revisited.esm`
	* `HeirApparent.esp`
	* `NotSoFast.esp`
	* `IntoTheDeepWoods.esp`
7. Fire up LOOT again an rearrange your load order, which will change due to the cleaning. This should be the deal:
	* `Fallout3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CALIBR.esm`
	* `Mart's Mutant Mod.esm`
	* `EVE.esm`
	* **`ArefuExpandedByAzar.esm`**
	* **`Mothership Crew.esm`**
	* `RH_IRONSIGHTS.esm`
	* **`TheInstitute.esm`**
	* **`Vault 101 Revisited.esm`**
	* **`Alton, IL.esm`**
	* `CRAFT.esm`
	* `FO3 Wanderers Edition - Main File.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `CASM.esp`
	* `BetterGamePerformance.esp`
	* `GNR Enhanced.esp`
	* `DarNifiedUIF3.esp`
	* **`AltonAddon.esp`**
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `Blackened FWE + MMM + EVE.esp`
	* `RH_FWE_Bridge.esp`
	* **`HeirApparent.esp`**
	* **`NotSoFast.esp`**
	* `WeaponModKits.esp`
	* `RH_EVE_Bridge.esp`
	* **`IntoTheDeepWoods.esp`**
	* `Existence 2.0.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `WeaponModKits - BrokenSteel.esp`
	* `WeaponModKits - OperationAnchorage.esp`
	* `WeaponModKits - ThePitt.esp`
	* `WeaponModKits - Zeta.esp`
	* `WeaponModKits - PointLookout.esp`
	* `RH_WMK_Bridge.esp`
	* **`ArefuExpandedByAzar-Radio.esp`**
	* `Conelrad 640-1240.esp`
	* **`FasterMorePowerfulMines.esp`**
8. Launch the game and wait a few moments to see several dialogs to kick-in the missions (except _Mothership Zeta Crew_, which launches elsewhere).
![Fallout 3 new quests dialog 1](Images/Fallout%203%20new%20quests%20dialog%201.png)
![Fallout 3 new quests dialog 2](Images/Fallout%203%20new%20quests%20dialog%202.png)
![Fallout 3 new quests dialog 3](Images/Fallout%203%20new%20quests%20dialog%203.png)
![Fallout 3 new quests dialog 4](Images/Fallout%203%20new%20quests%20dialog%204.png)
9. You can check the quests pulling up your Pip-Boy and navigating to the _Data_ section, _Notes_ option. The following notes should be there for you:
![Fallout 3 new quests notes](Images/Fallout%203%20new%20quests%20notes.png)


#### <a id="gearFallenBrother"></a>4.4.2. Gear for a fallen brother

Gopher has created four mods which add an interesting gear set based on a fallen Brotherhood of Steel's operative. These mods are:

* [_Advanced Recon Stealth Armor_](http://www.nexusmods.com/fallout3/mods/2654/)
* [_Advanced Recon Trap Detection_](http://www.nexusmods.com/fallout3/mods/15641/)
* [_Advanced Recon Range Finder_](http://www.nexusmods.com/fallout3/mods/15744/)
* [_Advanced Recon Thermal Nightvision_](http://www.nexusmods.com/fallout3/mods/15653/)

There is a small Gopher's video showing the [features of the Advanced Recon gear set](https://www.youtube.com/watch?v=OsstmRso_Jw) (4:42).

Let's install them:

1. Download _Advanced Recon Armor v 4_ from [_Advanced Recon Stealth Armor_](http://www.nexusmods.com/fallout3/mods/2654/) with NMM.
2. Download _Detect Traps v 2_ and _Adv Recon Thermal Nightvision - Detect Traps Patch_ from [_Advanced Recon Trap Detection_](http://www.nexusmods.com/fallout3/mods/15641/) with NMM.
3. Download _Adv Recon Range Finder_ from [_Advanced Recon Range Finder_](http://www.nexusmods.com/fallout3/mods/15744/) with NMM.
4. Download _Adv Recon Thermal Nightvision_, _Mr Burkes key_ and _Adv Recon Thermal Nightvision - FWE Patch_ from [_Advanced Recon Thermal Nightvision_](http://www.nexusmods.com/fallout3/mods/15653/) with NMM.
5. There is an interesting patch which [enables nightvision/thermalvision on any headgear](http://www.nexusmods.com/fallout3/mods/20806/), not limited to Advanced Recon Armor. Download _Advanced Recon Patcher_ with NMM.
5. You should have the complete _Advanced Recon_ set by now.
![NMM Advanced Recon set](Images/NMM%20Advanced%20Recon%20set.png)
6. Activate the mods in the following order.
	* _Advanced Recon Stealth Armor_
	* _Advanced Recon Trap Detection - Detect Traps v 2_
	* _Advanced Recon Range Finder FO3 - Adv Recon Range Finder_
	* _Advanced Recon Thermal Nightvision - Adv Recon Thermal Nightvision_
	* _Advanced Recon Thermal Nightvision - Mr Burkes key_
	* _Advanced Recon Trap Detection - Adv Recon Thermal Nightvision - Detect Traps Patch_
	* _Advanced Recon Thermal Nightvision Patcher - Advanced Recon Patcher_
	* _Advanced Recon Thermal Nightvision - Adv Recon Thermal Nightvision - FWE Patch_
7. When you activate _Advanced Recon Stealth Armor_, a pop-up with options will, well, pop up. Leave the options unchanged and click on _Install_.
![NMM Advanced Recon Stealth Armor install options](Images/NMM%20Advanced%20Recon%20Stealth%20Armor%20install%20options.png)
8. When you activate _Advanced Recon Thermal Nightvision - Adv Recon Thermal Nightvision_, NMM asks for permission to overwrite files from the previous iHUD installation. It adds certain overlay items when using scopes and binoculars. Answer _Yes to all_, as usual.
![NMM Advanced Recon Range Finder overwrite](Images/NMM%20Advanced%20Recon%20Range%20Finder%20overwrite.png)
9. Fire up LOOT to rearrange your load order. This should be your mod stack:
	* `Fallout3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CALIBR.esm`
	* `Mart's Mutant Mod.esm`
	* `EVE.esm`
	* `ArefuExpandedByAzar.esm`
	* `Mothership Crew.esm`
	* `RH_IRONSIGHTS.esm`
	* `TheInstitute.esm`
	* `Vault 101 Revisited.esm`
	* `Alton, IL.esm`
	* `CRAFT.esm`
	* `FO3 Wanderers Edition - Main File.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* **`Detect Traps.esm`**
	* **`Advanced Recon Tech.esm`**
	* `CASM.esp`
	* `BetterGamePerformance.esp`
	* `GNR Enhanced.esp`
	* `DarNifiedUIF3.esp`
	* `AltonAddon.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `Blackened FWE + MMM + EVE.esp`
	* `RH_FWE_Bridge.esp`
	* `HeirApparent.esp`
	* `NotSoFast.esp`
	* `WeaponModKits.esp`
	* `RH_EVE_Bridge.esp`
	* `IntoTheDeepWoods.esp`
	* `Existence 2.0.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `WeaponModKits - BrokenSteel.esp`
	* `WeaponModKits - OperationAnchorage.esp`
	* `WeaponModKits - ThePitt.esp`
	* `WeaponModKits - Zeta.esp`
	* `WeaponModKits - PointLookout.esp`
	* `RH_WMK_Bridge.esp`
	* `ArefuExpandedByAzar-Radio.esp`
	* `Conelrad 640-1240.esp`
	* `FasterMorePowerfulMines.esp`
	* **`Advanced Recon Gear.esp`**
	* **`Advanced Recon Armor.esp`**
	* **`Detect Traps - Perk.esp`**
	* **`Detect Traps - The Traponator 4000.esp`**
	* **`Detect Traps - DLC.esp`**
	* **`Advanced Recon Range Finder.esp`**
	* **`Advanced Recon Tech.esp`**
	* **`Advanced Recon Tech - Detect Traps.esp`**
	* **`Advanced Recon Equipment Patcher.esp`**
	* **`Advanced Recon Tech FWE.esp`**
10. Launch the game and check your new nice looking outfit. In your Pip-Boy (section _Items_, option _Apparel_), there are two new options to configure your Advanced Recon gear settings.
![Fallout 3 Advanced Recon black coat](Images/Fallout%203%20Advanced%20Recon%20black%20coat.png)
![Fallout 3 Advanced Recon gear settings](Images/Fallout%203%20Advanced%20Recon%20gear%20settings.png)


#### <a id="achievementJunkie"></a>4.4.3. For the achievement junkie in you

If you have ever played _World of Warcraft_, you will know that there is a deep, ingrained part of your reptilian brain that generates a huge amount of endorphines every time you get an _Achievement unlocked_ message after fulfilling a series of tasks.

I know what I am talking about. Trust me.

Well, _there are_ achievements in _Fallout 3_, but they are not clearly visible after their first (and only) appearance. [This mod](http://www.nexusmods.com/fallout3/mods/11326/) (and [its fix](http://www.nexusmods.com/fallout3/mods/18678/)) lets you view all your achievements in the _Data_/_Notes_ section of your Pip-Boy. However, be advised: the log gets installed only in a fresh playthrough, using the main Vault 101 start, not one of the alternate starts from FWE.

1. Download _Personal Achievements Log v12_ from [_Personal Achievements Log_](http://www.nexusmods.com/fallout3/mods/11326/) with NMM.
2. Download _SeraphTCs Personal Achievements Log FIX_ from [_SeraphTCs Personal Achievements Log FIX_](http://www.nexusmods.com/fallout3/mods/18678/) with NMM.
3. Activate the mods in the same order you downloaded them. The fix should overwrite files from the main mod, as usual.
4. The mod installs a number of `.esp` files, but we don't need all of them. Since we are using the GOTY version of _Fallout 3_, we only need `PAL - MERGED.esp`, so open the data folder (`[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data]`) and delete the following files:
	* `PAL - BASE File.esp`
	* `PAL - Broken Steel.esp`
	* `PAL - Mothership Zeta.esp`
	* `PAL - Operation Anchorage.esp`
	* `PAL - Point Lookout.esp`
	* `PAL - The Pitt.esp`
5. Run LOOT to rearrange your load order:
	* `Fallout3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CALIBR.esm`
	* `Mart's Mutant Mod.esm`
	* `EVE.esm`
	* `ArefuExpandedByAzar.esm`
	* `Mothership Crew.esm`
	* `RH_IRONSIGHTS.esm`
	* `TheInstitute.esm`
	* `Vault 101 Revisited.esm`
	* `Alton, IL.esm`
	* `CRAFT.esm`
	* `FO3 Wanderers Edition - Main File.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `Detect Traps.esm`
	* `Advanced Recon Tech.esm`
	* `CASM.esp`
	* `BetterGamePerformance.esp`
	* `GNR Enhanced.esp`
	* `DarNifiedUIF3.esp`
	* `AltonAddon.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `Blackened FWE + MMM + EVE.esp`
	* `RH_FWE_Bridge.esp`
	* `HeirApparent.esp`
	* `NotSoFast.esp`
	* `WeaponModKits.esp`
	* `RH_EVE_Bridge.esp`
	* `IntoTheDeepWoods.esp`
	* `Existence 2.0.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `WeaponModKits - BrokenSteel.esp`
	* `WeaponModKits - OperationAnchorage.esp`
	* `WeaponModKits - ThePitt.esp`
	* `WeaponModKits - Zeta.esp`
	* `WeaponModKits - PointLookout.esp`
	* `RH_WMK_Bridge.esp`
	* `ArefuExpandedByAzar-Radio.esp`
	* `Conelrad 640-1240.esp`
	* `FasterMorePowerfulMines.esp`
	* `Advanced Recon Gear.esp`
	* `Advanced Recon Armor.esp`
	* `Detect Traps - Perk.esp`
	* `Detect Traps - The Traponator 4000.esp`
	* `Detect Traps - DLC.esp`
	* `Advanced Recon Range Finder.esp`
	* `Advanced Recon Tech.esp`
	* `Advanced Recon Tech - Detect Traps.esp`
	* `Advanced Recon Equipment Patcher.esp`
	* `Advanced Recon Tech FWE.esp`
	* **`PAL - MERGED.esp`**
6. You will have to start a fresh game to see the achievements log in action. At your ninth birthday party, when you receive your own Pip-Boy from the hands of the Overseer,  navigate through the _Data_ button, _Notes_ option. There should be a _Personal achievements Log_ option to view your short achievement list (at least for the time being).
![Fallout 3 personal achievements log](Images/Fallout%203%20personal%20achievements%20log.png)



### <a id="takeOverTheWorkd"></a>4.5. So you want to take over the world, uh?

Who has not ever dreamed of taking over the world with an army of half-crazed human-killing robots manufactured by oneself?

Well, I have. Sort of.

But let's talk about robots in _Fallout 3_. By now, you have seen them. They are ubiquitous, and if you mess with them, you will end up being some hundred degrees more roasted than usual. To begin with.

However, they are just NPCs. Rusty, metal-ass NPCs, but NPCs nonetheless. You can't create new robots, and you can't command existing ones either.

Until [_RobCo Certified_](http://www.nexusmods.com/fallout3/mods/712/) appeared, that is.

With this mod you get a new perk which gives you the ability to repair destroyed robots or create new ones out of scrap collected throughout your wanderings. The wet dream of you, brother nerds. You can take a peek at the video [showcasing some of the mod features](https://www.youtube.com/watch?v=47sbkmImwDE) (1:03), by TheTalkieToaster, the mod author.

This mod requires a bit of fiddling because it's not ready to work along the Paradox version of [_EVE_](http://www.nexusmods.com/fallout3/mods/8340/?), so we need to install a patch and make sure the right files are in place. Let's get on with it.

1. Download the following files from [_RobCo Certified_](http://www.nexusmods.com/fallout3/mods/712/) manually, in a folder of your choice (say, `[%ROBCO_FULL%]`):
	* [_RobCo Certified v2_](http://www.nexusmods.com/fallout3/download/81129)
	* [_CuteUnits Side Mod_](http://www.nexusmods.com/fallout3/download/75621)
	* [_RobCo Certified Mechanists Edition v2-01_](http://www.nexusmods.com/fallout3/download/71514)
	* [_RobCo Certified v2 Patch Pack v1-41_](http://www.nexusmods.com/fallout3/download/75619)
2. Unzip all four files into `[%ROBCO_FULL%]`. There will be no files with the same name.
3. Delete the following files inside `[%ROBCO_FULL%]`:
	* `RobCo Certified v2 EVE.esp`
	* `RobCo Certified v2 FWE.esp`
	* `RobCo Certified v2 Omnipatch.esp`
	* `RobCo Certified v2 Version Updater.esp`
	* `RobCo Certified v2 Zeta Addon.esp`
4. Zip the contents of `[%ROBCO_FULL%]` into a file named `RobCo Certified v2.zip`.
5. Fire up NMM and manually add `RobCo Certified v2.zip` in the _Mods_ tab.
6. Download _RobCo Certified Omnipatch for Paradox EVE_ from [_EVE - Energy Visuals Enhanced_](http://www.nexusmods.com/fallout3/mods/8340/) with NMM.
7. Download _Impervious Power Armour v2-2_ from [_Impervious Power Armour_](http://www.nexusmods.com/fallout3/mods/13325/) to add a stronger armour-plating to robots, impervious to small guns (it will also work with power armors for your character).
8. Download _Mister Smiths Scrapyard_ from [_Mr Smiths Scrapyard_](http://www.nexusmods.com/fallout3/mods/14075/) to get a vendor specialized in robot parts and junk.
9. We have all the files we need in NMM, locked and loaded.
![NMM RobCo mods installed](Images/NMM%20RobCo%20mods%20installed.png)
10. Activate the files in the following order, answering _Yes to all_ when asked to overwrite files:
	* _RobCo Certified v2_
	* _EVE - Energy Visuals Enhanced - RobCo Certified Omnipatch for Paradox EVE_
	* _Impervious Power Armour - Impervious Power Armour v2-2_
	* _Mr Smiths Scrapyard - Mister Smiths Scrapyard_
11. Run LOOT to rearrange your load order, which should be like this:
	* `Fallout3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CALIBR.esm`
	* `Mart's Mutant Mod.esm`
	* `EVE.esm`
	* `ArefuExpandedByAzar.esm`
	* `Mothership Crew.esm`
	* `RH_IRONSIGHTS.esm`
	* `TheInstitute.esm`
	* `Vault 101 Revisited.esm`
	* `Alton, IL.esm`
	* `Advanced Recon Tech.esm`
	* **`Companion Core.esm`**
	* **`RobCo Certified v2.esm`**
	* `CRAFT.esm`
	* `FO3 Wanderers Edition - Main File.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `Detect Traps.esm`
	* **`Impervious Power Armour.esm`**
	* `CASM.esp`
	* `BetterGamePerformance.esp`
	* `GNR Enhanced.esp`
	* `DarNifiedUIF3.esp`
	* `AltonAddon.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `Blackened FWE + MMM + EVE.esp`
	* `RH_FWE_Bridge.esp`
	* `HeirApparent.esp`
	* **`RobCo Certified v2 Omnipatch.esp`**
	* **`Mr Smith's Scrapyard.esp`**
	* `NotSoFast.esp`
	* `WeaponModKits.esp`
	* `RH_EVE_Bridge.esp`
	* `IntoTheDeepWoods.esp`
	* `Existence 2.0.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `WeaponModKits - BrokenSteel.esp`
	* `WeaponModKits - OperationAnchorage.esp`
	* `WeaponModKits - ThePitt.esp`
	* `WeaponModKits - Zeta.esp`
	* `WeaponModKits - PointLookout.esp`
	* `RH_WMK_Bridge.esp`
	* `ArefuExpandedByAzar-Radio.esp`
	* `Conelrad 640-1240.esp`
	* `FasterMorePowerfulMines.esp`
	* `Advanced Recon Gear.esp`
	* `Advanced Recon Armor.esp`
	* `Detect Traps - Perk.esp`
	* `Detect Traps - The Traponator 4000.esp`
	* `Detect Traps - DLC.esp`
	* `Advanced Recon Range Finder.esp`
	* `Advanced Recon Tech.esp`
	* `Advanced Recon Tech - Detect Traps.esp`
	* `Advanced Recon Equipment Patcher.esp`
	* `Advanced Recon Tech FWE.esp`
	* `PAL - MERGED.esp`
	* **`RobcoCertified24SideMod.esp`**
	* **`RobCo Certified v2 Impervious FWE.esp`**
	* **`RobCo Certified v2 Impervious.esp`**
	* **`RobCo Certified v2 Mechanist's Edition.esp`**
	* **`Companion Core DLC Addon.esp`**
12. There are four dirty files in our mod stack. Clean them up with FO3Edit, as usual:
	* `Companion Core.esm`
	* `RobCo Certified v2.esm`
	* `RobcoCertified24SideMod.esp`
	* `Companion Core DLC Addon.esp`
13. When you level up, you will get the RobCo Certified perk for you to unleash your nerdy urges.
![Fallout 3 RobCo Certified perk](Images/Fallout%203%20RobCo%20Certified%20perk.png)




## <a id="unveilingRealWasteland"></a>5. Unveiling the real Wasteland

_Fallout 3_ is a terrific game, but it shows its age at first sight. Moreover, the greenish tint that pervades everything is, by far, one of the most questionable design decisions Bethesda made, at least graphics-wise.

If you have followed this guide up to this point, you could play a greatly enjoyable game just with the mods I have recommended. But if you want to go the extra mile and change your visual perception of the Wasteland forever, please, be my guest and keep on reading.

However, be advised: the mods in this section will push your machine capabilities to the limit.


### <a id="sheWalksInBeauty"></a>5.1. She walks in beauty, like the night of cloudless climes and starry skies

One of the first things we can improve regarding the appearance of our world is the night sky. There are two mods ([_Enhanced Night Sky_](http://www.nexusmods.com/fallout3/mods/442/) and [_krzymar HI-RES Moon_](http://www.nexusmods.com/fallout3/mods/538/)) that will make you cry tears of joy every time you look up to the Moon.

That will also grant you a short lifespan, killed by any night-crawling creature which happens to find you an easy meal, ready to be disemboweled.

1. Download _Enhanced Night Sky_ file with NMM.
2. Download _krzymar_HI-RES_Moon-0_2_0-bright_ file with NMM (I prefer the brighter version, instead of the darker one).
3. Activate them in the same order you downloaded them. There shouldn't be any overwriting. There are no data files installed either, so no need to run LOOT.
4. Launch the game and just compare.
![Fallout 3 night before](Images/Fallout%203%20night%20before.png)
![Fallout 3 night after](Images/Fallout%203%20night%20after.png)



### <a id="uncannyNuclearHolocaust"></a>5.2. The Nuclear Holocaust like you have never seen before

One of the things I like less of the visual aspect of the game is the green tint that paints everything. I guess that is supposed to depict the residual haze from a nuclear holocaust, but I don't like it anyway.

There is a single mod that not only removes the green tint, but also adds an incredible look to the game and a weather system: [_Project Reality_](http://www.nexusmods.com/fallout3/mods/17418/). No more fixed skin-burning sunny days for the Capital Wasteland.

Gopher has a video which covers different [weather and lighting mods available](https://www.youtube.com/watch?v=oHariRMIryI) (14:56), including _Project Reality_. However, we are going to tinker with the mod file because there is apparently a significant framerate drop with the default rain textures. We are going to replace them with [_Enhanced weather_](http://www.nexusmods.com/fallout3/mods/6170/) rain textures.

1. Download _F3ProjectRealityMkI_ manually, **NOT** with NMM.
2. Download _RECCOMANDED Enhanced Weather - Rain and Snow v2 hotfix b Fomod Package- FULL DO NOT DOWNLOAD ANYTHING ELSE_ manually, **NOT** with NMM.
3. Uncompress `RECCOMANDED Enhanced Weather - Rain and Snow v2  hotfix b Fomod Package- FULL DO NOT DOWNLOAD ANYTHING ELSE-6170.zip` in a location of your choice. The ZIP contains a single file, `Enhanced Weather - Rain and Snow v2 hotfix b.fomod`.
4. Using 7-zip or any other unzipping tool, extract the contents of `Enhanced Weather - Rain and Snow v2 hotfix b.fomod` to a location of your choice, namely `[%ENHANCED_WEATHER%]`.
5. Uncompress `F3ProjectRealityMkI-17418-v1-0beta.rar` in a location of your choice, namely `[%PROJECT_REALITY%]`.
6. Browse to `[%ENHANCED_WEATHER%\Textures\Mieimod\Different Weather]`, and copy these two files to `[%PROJECT_REALITY%\\textures\F3NV\Weather]`:
	* `Rain.dds`
	* `Rain2.dds`
![Fallout 3 Project Reality with enhanced weather textures](Images/Fallout%203%20Project%20Reality%20with%20enhanced%20weather%20textures.png)
7. Now, remove the following files from that folder:
	* `F3NVRain.dds`
	* `F3NVRain2.dds`
8. Rename the _Enhanced Weather_ files as follows:
	* `Rain.dds` &rarr; `F3NVRain.dds`
	* `Rain2.dds` &rarr; `F3NVRain2.dds`
9. Re-zip the contents of the `[%PROJECT_REALITY%]` folder into an archive named `F3ProjectRealityMkI-17418-v1-0beta-retextured.7z`
10. Open NMM and click on the green plus sign in the left button bar to manually add the file we just created.
![NMM install mod from file](Images/NMM%20install%20mod%20from%20file.png)
11. When the file is loaded, select it and click on the info button to change the name to "F3ProjectRealityMkI retextured".
![NMM renaming Project Reality](Images/NMM%20renaming%20Project%20Reality.png)
12. Double-click on the mod's name to activate it. There shouldn't be any overwriting.
13. Launch LOOT to rearrange your load order.
	* `Fallout3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CALIBR.esm`
	* `Mart's Mutant Mod.esm`
	* `EVE.esm`
	* `ArefuExpandedByAzar.esm`
	* `Mothership Crew.esm`
	* `RH_IRONSIGHTS.esm`
	* `Alton, IL.esm`
	* `CRAFT.esm`
	* `FO3 Wanderers Edition - Main File.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `Detect Traps.esm`
	* `Advanced Recon Tech.esm`
	* `CASM.esp`
	* `DarNifiedUIF3.esp`
	* `AltonAddon.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `HZSmoothLight - FO3.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `Blackened RH + FWE + EVE.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `WeaponModKits.esp`
	* `WeaponModKits - BrokenSteel.esp`
	* `WeaponModKits - OperationAnchorage.esp`
	* `WeaponModKits - Zeta.esp`
	* `WeaponModKits - ThePitt.esp`
	* `WeaponModKits - PointLookout.esp`
	* **`F3ProjectRealityMkI.esp`**
	* `ArefuExpandedByAzar-Radio.esp`
	* `Advanced Recon Gear.esp`
	* `Advanced Recon Armor.esp`
	* `Detect Traps - Perk.esp`
	* `Detect Traps - The Traponator 4000.esp`
	* `Detect Traps - DLC.esp`
	* `Advanced Recon Range Finder.esp`
	* `Advanced Recon Tech.esp`
	* `Advanced Recon Tech - Detect Traps.esp`
	* `Advanced Recon Equipment Patcher.esp`
	* `Advanced Recon Tech FWE.esp`
	* `PAL - MERGED.esp`
14. Launch the game and check the incredible look the Wasteland just got!
![Fallout 3 Project Reality installed](Images/Fallout%203%20Project%20Reality%20installed.png)
15. Pull up your PipBoy to check the new option in _Items_/_Apparel_ section to configure _Project Reality_.
![Fallout 3 Project Reality option](Images/Fallout%203%20Project%20Reality%20option.png)
16. Click on _Project Reality MkI_ and check the settings. There are a lot of things for you to tinker with until you feel comfortable (or uncomfortable, since I guess radioactive rain is not a pretty thing to be under).
![Fallout 3 Project Reality settings](Images/Fallout%203%20Project%20Reality%20settings.png)

Just a small note... Remember the previous screenshot showing our enhanced night? Well, look at this:

![Fallout 3 night after Project Reality](Images/Fallout%203%20night%20after%20Project%20Reality.png)

Things keep getting better and better!



### <a id="pointOfView"></a>5.3. Everything depends on the point of view

At first, I didn't think to include these four mod in this guide:

* [_CINEMATECH_](http://www.nexusmods.com/fallout3/mods/15745/)
* [_Director's Chair_](http://www.nexusmods.com/fallout3/mods/17899/)
* [_Dynavision_](http://fallout3.nexusmods.com/mods/17876/)
* [_The IMAGINATOR_](http://www.nexusmods.com/fallout3/mods/16875/)

I only considered _Dynavision_ worth installing, but after revisiting Gopher's video about [visual enhancements mods](https://www.youtube.com/watch?v=ry-84eqDvr0) (29:59), I changed my mind, not only because the customization possibilities of the combined mods, but also because you don't even need the Pip-Boy menu to change the settings of the mods (specially _Dynavision_). That's a great plus.

These four mods give you total control about light. And no, these are not lighting mods (we'll be there [in a breeze](#letThereBeLight)). These are mods to _control_ the way the light behaves in your game.

Let me explain. At a very basic level, every game lets you customize three parameters: brightness, contrast and saturation. However, the sum of the aforementioned mods let you control the kind of light, the "film grain" and even the depth of field of your point of view.

Let's get started.

1. Download _DYNAVISION - Dynamic Lens Effect 1\_0\_1_ with NMM.
2. Download _CINEMATECH_ with NMM.
3. Download _The IMAGINATOR for FO3 - Visual Control Device_ with NMM.
4. Download _Directors Chair_ with NMM.
5. We should have the four mods downloaded in no time.
![NMM visual enhancements downloaded](Images/NMM%20visual%20enhancements%20downloaded.png)
6. Activate _DYNAVISION - Dynamic Depth of Field - DYNAVISION - Dynamic Lens Effect 1\_0\_1_ by double-clicking on it. No overwriting is required.
7. Activate _CINEMATECH - Film Grains and Styles - CINEMATECH_ the same way. It will ask you to overwrite a HUD file previously installed by _Advanced Recon Thermal Nightvision_. Go on and answer _Yes to all_.
8. Activate _The IMAGINATOR for FO3 - Visual Control Device - The IMAGINATOR for FO3 - Visual Control Device_ the same way. No overwriting required.
9. Finally, activate _Directors Chair - Total Visual Control - Directors Chair_. No overwriting either.
10. Fire up LOOT to rearrange your load order. This should be the deal.
	* `Fallout3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CALIBR.esm`
	* `Mart's Mutant Mod.esm`
	* `EVE.esm`
	* `ArefuExpandedByAzar.esm`
	* `Mothership Crew.esm`
	* `RH_IRONSIGHTS.esm`
	* `Alton, IL.esm`
	* `CRAFT.esm`
	* `FO3 Wanderers Edition - Main File.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `Detect Traps.esm`
	* `Advanced Recon Tech.esm`
	* **`CINEMATECH.esm`**
	* **`ImaginatorFO3.esp`**
	* `CASM.esp`
	* `DarNifiedUIF3.esp`
	* `AltonAddon.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `HZSmoothLight - FO3.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `Blackened RH + FWE + EVE.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `WeaponModKits.esp`
	* `WeaponModKits - BrokenSteel.esp`
	* `WeaponModKits - OperationAnchorage.esp`
	* `WeaponModKits - Zeta.esp`
	* `WeaponModKits - ThePitt.esp`
	* `WeaponModKits - PointLookout.esp`
	* `F3ProjectRealityMkI.esp`
	* `ArefuExpandedByAzar-Radio.esp`
	* `Advanced Recon Gear.esp`
	* `Advanced Recon Armor.esp`
	* `Detect Traps - Perk.esp`
	* `Detect Traps - The Traponator 4000.esp`
	* `Detect Traps - DLC.esp`
	* `Advanced Recon Range Finder.esp`
	* `Advanced Recon Tech.esp`
	* `Advanced Recon Tech - Detect Traps.esp`
	* `Advanced Recon Equipment Patcher.esp`
	* `Advanced Recon Tech FWE.esp`
	* `PAL - MERGED.esp`
	* **`DYNAVISION - Dynamic Lens Effect.esp`**
	* **`Directors Chair - Fallout 3.esp`**
11. Launch the game to check the new menus. Pressing <kbd>F7</kbd> will show the _Director's Chair_ in-game menu. The best way to get the grasp of the possibilities given by these four mods is watching Gopher's video.
![Fallout 3 Director's Chair](Images/Fallout%203%20Director's%20Chair.png)



### <a id="beautifulSkin"></a>5.4. A beautiful skin

_Fallout 3_ was released in 2008... and it really shows its age when you look at it more than two whole seconds.

Old graphics shouldn't be an issue with a game like this, but when you see how the game improves with new textures... Well, you will never be able to play the vanilla version again. Ever.

Be advised though: these mods will push your rig capabilities to its limits. Gopher explains the different flavours of textures you can install in the [visual enhancements mods](https://www.youtube.com/watch?v=ry-84eqDvr0) (29:59) we saw earlier, although he covers just _NMCS Texture Pack_.

These are the mods we are going to install:

* [_Flora Overhaul_](http://www.nexusmods.com/fallout3/mods/19864/)
* [_NMCS Texture Pack_](http://www.nexusmods.com/fallout3/mods/12056/)
* [_Pure Water_](http://www.nexusmods.com/fallout3/mods/2599/)
* [_Clean-Deluxe_](http://www.nexusmods.com/fallout3/mods/17115/)

We are not going to use the full version of _NMCS Texture Pack_ because the performance version is just about as good. Regarding to _Flora Overhaul_, I prefer the _Dead Edition_ because, you know, a Wasteland full of trees cannot barely considered a wasteland anymore. However, feel free to ignore me (why the hell are you reading this, anyway?).

Finally, _Pure Water_ removes the muddy aspect of the water (but not its radiation, although it's optional, too), and _Clean-Deluxe_ will give us a 5-10% improvement in FPS, removing clutter and atmospheric haze which, in fact, add nothing meaningful to the game.

Let's begin!

1. Download _NMCs Texture Pack PERFORMANCE Pack SINGLE FILE FOR NMM_ with NMM. Go partying the whole night while this mod is downloaded.
2. Download _Dead Edition v13C_ with NMM.
3. Download _PureWater_ with NMM.
4. Download _Clean-Deluxe GOTY Edition_ with NMM.
5. We have our 4 mods downloaded and ready to be installed.
![NMM texture mods](Images/NMM%20texture%20mods.png)
6. Activate _NMCs\_Texture\_Pack\_for\_FO3 - NMCs Texture Pack PERFORMANCE Pack SINGLE FILE FOR NMM_ double-clicking on it. No overwriting required, as this mods comprises just textures.
7. Activate _FO3 Flora Overhaul - Dead Edition v13C_ double-clicking on it. Again, no overwriting required.
8. Activate _PureWater - PureWater_. No overwriting required.
9. Activate _Clean-Deluxe - Clean-Deluxe GOTY Edition_. No overwriting required.
10. _Pure Water_ comes in four flavours, each one with its own `.esp` file:
	* `PureWater-VeryClearNoRad-.esp`: High water transparency and no radiation poisoning.
	* `PureWater-VeryCleanLittleRad-.esp`: High water transparency and radiation poisoning.
	* `PureWater-NoRad-.esp`: Normal water transparency and no radiation poisoning.
	* `PureWater-LittleRad-.esp`: Normal water transparency and radiation poisoning.
11. I am going to use high water transparency and radiation poisoning (`PureWater-VeryCleanLittleRad-.esp`), because, what could be better than a sip of plutonium-loaded clear water from the Potomac? We need to delete the unused files in `[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data]`.
12. Run LOOT to rearrange your load order, as usual.
	* `Fallout3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CALIBR.esm`
	* `Mart's Mutant Mod.esm`
	* `EVE.esm`
	* `ArefuExpandedByAzar.esm`
	* `Mothership Crew.esm`
	* `RH_IRONSIGHTS.esm`
	* `Alton, IL.esm`
	* `CRAFT.esm`
	* `FO3 Wanderers Edition - Main File.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `Detect Traps.esm`
	* `Advanced Recon Tech.esm`
	* `CINEMATECH.esm`
	* `ImaginatorFO3.esp`
	* `CASM.esp`
	* `DarNifiedUIF3.esp`
	* `AltonAddon.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* **`Clean-Deluxe GOTY.esp`**
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `Blackened RH + FWE + EVE.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `WeaponModKits.esp`
	* `WeaponModKits - BrokenSteel.esp`
	* `WeaponModKits - OperationAnchorage.esp`
	* `WeaponModKits - Zeta.esp`
	* `WeaponModKits - ThePitt.esp`
	* `WeaponModKits - PointLookout.esp`
	* `F3ProjectRealityMkI.esp`
	* `ArefuExpandedByAzar-Radio.esp`
	* `Advanced Recon Gear.esp`
	* `Advanced Recon Armor.esp`
	* `Detect Traps - Perk.esp`
	* `Detect Traps - The Traponator 4000.esp`
	* `Detect Traps - DLC.esp`
	* `Advanced Recon Range Finder.esp`
	* `Advanced Recon Tech.esp`
	* `Advanced Recon Tech - Detect Traps.esp`
	* `Advanced Recon Equipment Patcher.esp`
	* `Advanced Recon Tech FWE.esp`
	* `PAL - MERGED.esp`
	* `DYNAVISION - Dynamic Lens Effect.esp`
	* `Directors Chair - Fallout 3.esp`
	* **`Flora Overhaul.esp`**
	* **`PureWater-VeryCleanLittleRad-.esp`**
11. Launch the game to see for yourself.
![Fallout 3 new textures and flora night](Images/Fallout%203%20new%20textures%20and%20flora%20night.png)
![Fallout 3 new textures and flora day](Images/Fallout%203%20new%20textures%20and%20flora%20day.png)

The quality of the textures is hard to miss, not to mention the fuckload of trees that are thrown to your face all of a sudden.

![Fallout 3 new textures](Images/Fallout%203%20new%20textures.png)



### <a id="letThereBeLight"></a>5.5. Let there be light!

Lighting in _Fallout 3_ is somewhat unnatural. You would think everyone in the Capital Wasteland has developed nightvision, because you can see perfectly in pitch black underground places. Not to mention the horrid HDR blooming you get when the game does not handle well multiple light sources.

The three following mods try to enhance lighting in _Fallout 3_.

* [_Darkened Interiors_](http://www.nexusmods.com/fallout3/mods/16935/)
* [_Fallout Street Lights_](http://www.nexusmods.com/fallout3/mods/8069/)
* [_Megaton Lighting Overhaul_](http://www.nexusmods.com/fallout3/mods/7875/)

_Darkened Interiors_ tries to give interiors a realistic lighting, with deep shadows and islands of light, which creates a scarier atmosphere. _Fallout Street Lights_ revamps, well, the street lights, creating light beams where there was just diffuse glows. Finally, _Megaton Lighting Overhaul_ adds lights in Megaton, the first settlement you are going to find in your wanderings around the Wasteland (you will spend quite a lot of time there).

1. Download _Darkened Interiors v0\_3_ with NMM.
2. Download _Fallout Street Lights Version 2_ with NMM.
3. Download _Megaton Lighting Overhaul_ with NMM.
4. These are small mods, so you will have them downloaded in a breeze.
![NMM Lighting mods](Images/NMM%20Lighting%20mods.png)
5. Activate them in the same order you downloaded them. Each mod has its own set of files, so no overwriting is required.
6. Yeah, you guessed. Run LOOT.
	* `Fallout3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* **`StreetLights.esm`**
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CALIBR.esm`
	* `Mart's Mutant Mod.esm`
	* `EVE.esm`
	* `ArefuExpandedByAzar.esm`
	* `Mothership Crew.esm`
	* `RH_IRONSIGHTS.esm`
	* `Alton, IL.esm`
	* `CRAFT.esm`
	* `FO3 Wanderers Edition - Main File.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `Detect Traps.esm`
	* `Advanced Recon Tech.esm`
	* `CINEMATECH.esm`
	* `ImaginatorFO3.esp`
	* `CASM.esp`
	* `DarNifiedUIF3.esp`
	* `AltonAddon.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* `Clean-Deluxe GOTY.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `Blackened RH + FWE + EVE.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* **`Xepha's Darkened Interiors.esp`**
	* `WeaponModKits.esp`
	* **`Xepha's Darkened Interiors - BS.esp`**
	* `WeaponModKits - BrokenSteel.esp`
	* `WeaponModKits - OperationAnchorage.esp`
	* `WeaponModKits - Zeta.esp`
	* `WeaponModKits - ThePitt.esp`
	* **`Xepha's Darkened Interiors - PL.esp`**
	* `WeaponModKits - PointLookout.esp`
	* `F3ProjectRealityMkI.esp`
	* `ArefuExpandedByAzar-Radio.esp`
	* `Advanced Recon Gear.esp`
	* `Advanced Recon Armor.esp`
	* `Detect Traps - Perk.esp`
	* `Detect Traps - The Traponator 4000.esp`
	* `Detect Traps - DLC.esp`
	* `Advanced Recon Range Finder.esp`
	* `Advanced Recon Tech.esp`
	* `Advanced Recon Tech - Detect Traps.esp`
	* `Advanced Recon Equipment Patcher.esp`
	* `Advanced Recon Tech FWE.esp`
	* `PAL - MERGED.esp`
	* `DYNAVISION - Dynamic Lens Effect.esp`
	* `Directors Chair - Fallout 3.esp`
	* `Flora Overhaul.esp`
	* `PureWater-VeryCleanLittleRad-.esp`
	* **`Xepha's Darkened Interiors - OA.esp`**
	* **`megalight.esp`**
7. LOOT informs us that the file `StreetLights.esm` contains identical to master records, so we need to clean it with FO3Edit. Follow the usual procedure, selecting only that file and letting FO3Edit load the dependencies for you.
8. Launch the game and take a stroll in the night.
![Fallout 3 new lighting](Images/Fallout%203%20new%20lighting.png)
![Fallout 3 Megaton entrance light](Images/Fallout%203%20Megaton%20entrance%20light.png)
![Fallout 3 Megaton street lights](Images/Fallout%203%20Megaton%20street%20lights.png)



### <a id="dontLikeYourFace"></a>5.6. I don't like your face

I guess no one is able to remember the moment of her birth, unless you are a trickster. However, I would be shitting bricks my whole life if my first sight in this world were these eyes.

![Fallout 3 WTF with your eyes](Images/Fallout%203%20WTF%20with%20your%20eyes.png)

Seriously, look at _that_.

![Fallout 3 WTF WTF WTF DADDY](Images/Fallout%203%20WTF%20WTF%20WTF%20DADDY.png)

A poor face modeling is one of the worst thing I can imagine to get a proper immersion in the game. Imagine your ninth birthday, surrounded by a bunch of people like this.

![Fallout 3 ugly faces](Images/Fallout%203%20ugly%20faces.png)

Consider the face of your childhood friend Amata, and take into account that hers is not the ugliest face you will encounter in the game.

![Fallout 3 Amata is not so ugly after all](Images/Fallout%203%20Amata%20is%20not%20so%20ugly%20after%20all.png)

The following mods target the faces, character animation and eye textures.

* [_Fallout 3 re-animated_](http://www.nexusmods.com/fallout3/mods/7670/)
* [_Fallout 3 redesigned_](http://www.nexusmods.com/fallout3/mods/6341/)
* [_Lost in Light_](http://www.nexusmods.com/fallout3/mods/19163/)

_Fallout 3 re-animated_ changes the default animations of every character in-game, getting a more natural stance, both in combat and resting. _Fallout 3 redesigned_, formerly known as _Project Beauty_, changes all the faces throughout the game, giving people a more natural look. Finally, _Lost in Light_ (LiL, for short) replaces the vanilla eye textures with proper eyeballs using proper light reflection. No more people screaming out their pain of their wretched souls through the eyes. As usual, Gopher has a video about [people reanimated and redesigned](https://www.youtube.com/watch?v=smLZNJIMCQA) (11:06), although he doesn't cover LiL.

The installation is a bit tricky, regarding to _Fallout 3 Redesigned_, so let's do it.

1. Download _Release v0\_22_ and _Idle Revisions2 - Fixed_ from _Fallout 3 re-animated_ with NMM.
2. Download _FO3 Redesigned HD_, but download it **manually**. We are going to meddle with the file a little. The file is named `FO3 Redesigned HD-6341-2-74-2.zip` (obviously, these instructions may not apply with a different version of the mod).
3. Download _Lost in Light - An Eye Improvement Mod_ with NMM.
4. Unzip `FO3 Redesigned HD-6341-2-74-2.zip` in a location of your choice, say `[%FO3_REDESIGNED%]`.
5. The structure of the ZIP file is a bit weird.
![FO3 Redesigned mod structure](Images/FO3%20Redesigned%20mod%20structure.png)
6. We are going to create a mod file with just the items we need, in the proper place. Create a folder anywhere you want, say `[%FO3_REDESIGNED_REPACK%]`.
7. Create the following folders under `[%FO3_REDESIGNED_REPACK%]`:
	* `Meshes`
	* `textures`
8. Copy the following files from `[%FO3_REDESIGNED%]` into `[%FO3_REDESIGNED_REPACK%]`:
	* `/meshes/*.*` &rarr; `/Meshes/`
	* `/textures/*.*` &rarr; `/textures/`
	* `/Optional Merged Version/Project Beauty.esm` &rarr; `/`
9. Zip the contents of the `[%FO3_REDESIGNED_REPACK%]` folder into a file named `FO3_REDESIGNED_REPACK.zip`. The folders `/Meshes/` and `/textures/` should be in the root of the ZIP file.
10. In NMM, use the option _Add Mod from File_ (green plus sign in the leftmost button bar) and select the newly created file.
11. We need one final thing to put all the pieces together. Remember the chapter about [weaponry](#weNeedMoreFirepower), when I told you about a Blackened patch we couldn't install yet? That was _Blackened FWE - MMM - EVE - Project Beauty_ file from [_Blackened_](http://www.nexusmods.com/fallout3/mods/18173/). Now it's the time to download it with NMM.
12. Ok, we have all the files we need, ready to be installed.
![NMM people redesigned and reanimated mods](Images/NMM%20people%20redesigned%20and%20reanimated%20mods.png)
13. Activate the mods in the following order:
	* _Fallout 3 Re-Animated - Release v0\_22_ (this one overwrites files from _RH\_IronSights_, so answer _Yes to all_ when asked to).
	* _Fallout 3 Re-Animated - Idle Revisions2 - Fixed_ (this one overwrites files from the previous file, so answer _Yes to all_ when asked to).
	* _FO3\_REDESIGNED\_REPACK_ (no overwriting required).
	* _LiL - An Eye Improvement Mod - Lost in Light - An Eye Improvement Mod_ (this one overwrites files from _Fallout 3 Redesigned_, so answer _Yes to all_ when asked to).
	* _Blackened - Blackened FWE - MMM - EVE - Project Beauty_ (this is a patch, so overwriting is expected; you know the drill).
14. Run LOOT to rearrange your load order. This should be it.
	* `Fallout3.esm`
	* `Anchorage.esm`
	* `ThePitt.esm`
	* `StreetLights.esm`
	* `BrokenSteel.esm`
	* `PointLookout.esm`
	* `Zeta.esm`
	* `Unofficial Fallout 3 Patch.esm`
	* `aHUD.esm`
	* `iHUD.esm`
	* `CALIBR.esm`
	* `Mart's Mutant Mod.esm`
	* **`Project Beauty.esm`**
	* `EVE.esm`
	* `ArefuExpandedByAzar.esm`
	* `Mothership Crew.esm`
	* `RH_IRONSIGHTS.esm`
	* `Alton, IL.esm`
	* `CRAFT.esm`
	* `FO3 Wanderers Edition - Main File.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `Detect Traps.esm`
	* `Advanced Recon Tech.esm`
	* `CINEMATECH.esm`
	* `ImaginatorFO3.esp`
	* `Flora Overhaul.esp`
	* `CASM.esp`
	* `DarNifiedUIF3.esp`
	* `AltonAddon.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* `Clean-Deluxe GOTY.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `Xepha's Darkened Interiors.esp`
	* `Xepha's Darkened Interiors - BS.esp`
	* `Xepha's Darkened Interiors - PL.esp`
	* **`Blackened FWE + MMM + EVE + Project Beauty.esp`**
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `Blackened RH + FWE + EVE.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `WeaponModKits.esp`
	* `WeaponModKits - BrokenSteel.esp`
	* `WeaponModKits - OperationAnchorage.esp`
	* `WeaponModKits - Zeta.esp`
	* `WeaponModKits - ThePitt.esp`
	* `WeaponModKits - PointLookout.esp`
	* `F3ProjectRealityMkI.esp`
	* `ArefuExpandedByAzar-Radio.esp`
	* `Advanced Recon Gear.esp`
	* `Advanced Recon Armor.esp`
	* `Detect Traps - Perk.esp`
	* `Detect Traps - The Traponator 4000.esp`
	* `Detect Traps - DLC.esp`
	* `Advanced Recon Range Finder.esp`
	* `Advanced Recon Tech.esp`
	* `Advanced Recon Tech - Detect Traps.esp`
	* `Advanced Recon Equipment Patcher.esp`
	* `Advanced Recon Tech FWE.esp`
	* `PAL - MERGED.esp`
	* `DYNAVISION - Dynamic Lens Effect.esp`
	* `Directors Chair - Fallout 3.esp`
	* `PureWater-VeryCleanLittleRad-.esp`
	* `Xepha's Darkened Interiors - OA.esp`
	* `megalight.esp`

Let's see how the game changes with this. What about the defining moment of your birth?

![Fallout 3 not so scary first sight](Images/Fallout%203%20not%20so%20scary%20first%20sight.png)

Well, it's a little bit les scary, although there are some remaining embers in these eyes.

![Fallout 3 embers in your eyes](Images/Fallout%203%20embers%20in%20your%20eyes.png)

There are certain improvements in the character customization options, although I don't quite get my own look-alike.

![Fallout 3 enhanced character customization](Images/Fallout%203%20enhanced%20character%20customization.png)

Let's check the bunch of people in your ninth birthday.

![Fallout 3 better faces](Images/Fallout%203%20better%20faces.png)

And what about Amata?

![Fallout 3 Amata has changed a bit](Images/Fallout%203%20Amata%20has%20changed%20a%20bit.png)

The changes are remarkable, as you can see by looking at before/after images side by side.




## <a id="wrappingUp"></a>6. Wrapping up

No matter which mods you have installed to this point, you will want to create a merged patch to ensure all of them work together like a charm.

Even with Bethesda's main files there are inconsistencies across the different DLCs, let alone with a fuckload of mods installed, each one with its own set of items and rules. A merged patch is no magic fix, but it is a good start point to solve certain basic problems that arise when different mods have different visions of the same issue. As usual, Gopher has [a video about FO3Edit](https://www.youtube.com/watch?v=uPK7R71zcwM) (39:12) which explains (from 14:05) what is a merged patch, how to create it and the things you will need to know about what it does and what it does not do.

1. Open FO3Edit and load **ALL** the plugins you have installed. This is important, as you are going to create a merged patch for your whole mod stack. Don't pay attention to the mods shown in the screenshots. Your mileage may vary.
![FO3Edit load all plugins](Images/FO3Edit%20load%20all%20plugins.png)
2. Wait until FO3Edit finishes loading all data files.
![FO3Edit background loader finished](Images/FO3Edit%20background%20loader%20finished.png)
3. Right-click anywhere in the leftmost panel (the one with the plugin list) and select _Other_, then _Create merged patch_.
![FO3 create merged patch](Images/FO3%20create%20merged%20patch.png)
4. Give the merged patch a meaningful name. I am using the version number of this guide, but you are free to choose whatever you like.
![FO3 merged patch name](Images/FO3%20merged%20patch%20name.png)
5. Check the leftmost panel at the bottom. Your merged patch should sit there.
![FO3Edit merged patch created](Images/FO3Edit%20merged%20patch%20created.png)
6. We need to exit FO3Edit to save the merged patch. Click on the _Close Window_ icon and make sure the merged patch is selected in the next window. Click _Ok_ to have the `.esp` file saved to your data folder.
![FO3Edit saving merged patch](Images/FO3Edit%20saving%20merged%20patch.png)
7. We need to activate the merged patch, so open NMM and navigate to the _Plugins_ tab. Tick the merged patch at the bottom, and you are good to go!
![NMM merged patch loaded](Images/NMM%20merged%20patch%20loaded.png)

Remember these golden rules regarding to merged patches:

1. A merged patch will not fix any inconsistency you have in your mod stack. As Gopher shows in the aforementioned video, a merged patch may, in fact, add some inconsistencies of its own (although they are minor ones). However, it will stitch together firmly the whole stack.
2. The merged patch should **ALWAYS** sit at the bottom of your load order. In case of conflict, the deepest mod always wins, so you need your merged patch sitting at the bottom to ensure proper conflict resolution.
3. As tedious as it sounds, every time you change your mod stack, adding or removing mods, you need to create a **NEW** merged patch. Otherwise, the game will miserably crash. As you can imagine, I have been creating _a lot_ of merged patches throughout the creation of this guide.




## <a id="resources"></a>7. Resources

This is a comprehensive list of the resources used throughout this guide.



### <a id="tools"></a>7.1. Tools

* [Nexus Mod Manager](http://www.nexusmods.com/games/mods/modmanager/). This is the tool of choice when it comes to keep all your mods organized and up-to-date.
* [LOOT](https://loot.github.io/). Installing mods on Bethesda games can be a pain in the ass, especially if you try to install a lot of possibly-colliding mods. This tool keeps the load order straight.
* [FO3Edit](http://www.nexusmods.com/fallout3/mods/637/). _Fallout 3_ itself comes out-of-the-box with certain errors in the main and DLC files, and this tool comes in handy to correct them. Besides, this is **THE** tool to create a merged patch to run the game with an absurd amount of mods.



### <a id="guides"></a>7.2. Guides

* [_Fallout 3_ Tweaking Guide](http://www.tweakguides.com/Fallout3_1.html).
* [Gamebryo console commands](http://fallout.wikia.com/wiki/Gamebryo_console_commands)
* [Guide to fix the game in order to run under modern versions of Windows](http://steamcommunity.com/sharedfiles/filedetails/id=149946772).
* [Item Codes](http://www.ign.com/wikis/fallout-3/Item_Codes)
* [Let's mod _Fallout 3_ with over 100 mods](http://www.gamingboulevard.com/2015/01/lets-mod-fallout-3-100-mods/)
* [TES5Edit cleaning guide](http://www.creationkit.com/index.php?title=TES5Edit_Cleaning_Guide_-_TES5Edit).
* [Why the game crashes if it runs in a box with multiple cores](http://www.sevenforums.com/gaming/20199-fallout-3-windows-7-w-quad-core.html).



### <a id="mods"></a>7.3. Mods

This is the list of mods used throughout this guide, in ascending alphabetical order.

|Mod|URL|
|---|---|
|_A Note Easily Missed_|http://www.nexusmods.com/fallout3/mods/4730/|
|_Adjustable HUD_|http://www.nexusmods.com/fallout3/mods/15886/|
|_Advanced Recon Range Finder_|http://www.nexusmods.com/fallout3/mods/15744/|
|_Advanced Recon Stealth Armor_|http://www.nexusmods.com/fallout3/mods/2654/|
|_Advanced Recon Thermal Nightvision Patcher_|http://www.nexusmods.com/fallout3/mods/20806/|
|_Advanced Recon Thermal Nightvision_|http://www.nexusmods.com/fallout3/mods/15653/|
|_Advanced Recon Trap Detection_|http://www.nexusmods.com/fallout3/mods/15641/|
|_Alton IL_|http://www.nexusmods.com/fallout3/mods/16949/|
|_Alton Revoiced lip files_|http://www.nexusmods.com/fallout3/mods/22041/|
|_Alton Revoicing Project_|http://www.nexusmods.com/fallout3/mods/20859/|
|_Ambient Wasteland 2_|http://www.nexusmods.com/fallout3/mods/12602/|
|_An Evening With Mister Manchester_|http://www.nexusmods.com/fallout3/mods/5630/|
|_Arefu Expanded_|http://www.nexusmods.com/fallout3/mods/8976/|
|_Beards of Fallout_|http://www.nexusmods.com/fallout3/mods/18622/|
|_Better Booze_|http://www.nexusmods.com/fallout3/mods/626/|
|_Better Game Performance_|http://www.nexusmods.com/fallout3/mods/13520/|
|_Better High Detail Map and Icons_|http://www.nexusmods.com/fallout3/mods/16898/|
|_Better HiRes Skill Books_|http://www.nexusmods.com/fallout3/mods/3876/|
|_Chems and Meds Re-Texture Pack_|http://www.nexusmods.com/fallout3/mods/15960/|
|_CINEMATECH_|http://www.nexusmods.com/fallout3/mods/15745/|
|_Clean-Deluxe_|http://www.nexusmods.com/fallout3/mods/17115/|
|_Community Ammunition Library_|http://www.nexusmods.com/fallout3/mods/3447/|
|_Darkened Interiors_|http://www.nexusmods.com/fallout3/mods/16935/|
|_Darnified UI_|http://forums.bethsoft.com/topic/1085562-wipzbeta-darnified-ui-f3/|
|_DCInteriors Project_|http://www.nexusmods.com/fallout3/mods/5573/|
|_Director’s Chair_|http://www.nexusmods.com/fallout3/mods/17899/|
|_Dynavision_|http://www.nexusmods.com/fallout3/mods/17876/|
|_Earth from Space texture for Mothership Zeta_|http://www.nexusmods.com/fallout3/mods/19294/|
|_Energy Visuals Enhanced_|http://www.nexusmods.com/fallout3/mods/8340/|
|_Enhanced Blood Textures v2_22b_|http://www.nexusmods.com/fallout3/mods/101/|
|_Enhanced Night Sky_|http://www.nexusmods.com/fallout3/mods/442/|
|_eXcalibr - ammo eXpansion pack_|http://www.nexusmods.com/fallout3/mods/11684/|
|_Existence 2_0 - Robot Radio_|http://www.nexusmods.com/fallout3/mods/5612/|
|_Expanded Megaton House V3_|http://www.nexusmods.com/fallout3/mods/2136/|
|_Fake Fullscreen Mode Windowed - Alt Tab Fix_|http://www.nexusmods.com/fallout3/mods/16001/|
|_Fallout 3 - Enhanced Camera_|http://www.nexusmods.com/fallout3/mods/20183/|
|_Fallout 3 - HD Audio Overhaul – v1.21_|http://www.nexusmods.com/fallout3/mods/13055/|
|_Fallout 3 Hirezd_|http://www.nexusmods.com/fallout3/mods/19931/|
|_Fallout 3 re-animated_|http://www.nexusmods.com/fallout3/mods/7670/|
|_Fallout 3 redesigned_|http://www.nexusmods.com/fallout3/mods/6341/|
|_Fallout 3 Wanderers Edition_|http://www.nexusmods.com/fallout3/mods/2761/|
|_Fallout Street Lights_|http://www.nexusmods.com/fallout3/mods/8069/|
|_Fallout Stutter Remover_|http://www.nexusmods.com/fallout3/mods/8886/|
|_Faster Pipboy Faster_|http://www.nexusmods.com/newvegas/mods/35225/|
|_Flora overhaul_|http://www.nexusmods.com/fallout3/mods/19864/|
|_FO3-WRP - Weapon Retexture Project_|http://www.nexusmods.com/fallout3/mods/18133/|
|_GNR Enhanced_|http://www.nexusmods.com/fallout3/mods/14946/|
|_Hall Of Equipment_|http://www.nexusmods.com/fallout3/mods/17145/|
|_HD Smoky Fire and Explosions for FO3_|http://www.nexusmods.com/fallout3/mods/20053/|
|_Hi-Res Weapons v3_|http://www.nexusmods.com/fallout3/mods/481/|
|_Immersive HUD_|http://www.nexusmods.com/fallout3/mods/15790/|
|_Impervious Power Armor_|http://www.nexusmods.com/fallout3/mods/13325/|
|_Improved Glass Bullet Impact_|http://www.nexusmods.com/fallout3/mods/13120/|
|_Improved LOD Noise Texture_|http://www.nexusmods.com/fallout3/mods/17743/|
|_Improved Sound FX v1.3_|http://www.nexusmods.com/fallout3/mods/627/|
|_krzymar HI-RES Moon_|http://www.nexusmods.com/fallout3/mods/538/|
|_Large Address Aware Enabler for Fallout 3_|http://www.nexusmods.com/fallout3/mods/6510/|
|_Lost in Light_|http://www.nexusmods.com/fallout3/mods/19163/|
|_Marts Mutant Mod_|http://www.nexusmods.com/fallout3/mods/3211/|
|_Megaton Lighting Overhaul_|http://www.nexusmods.com/fallout3/mods/7875/|
|_Megaton Walkway_|http://www.nexusmods.com/fallout3/mods/8247/|
|_Mothership Zeta Crew_|http://www.nexusmods.com/fallout3/mods/8747/|
|_Mothership Zeta DLC Retextured_|http://www.nexusmods.com/fallout3/mods/8260/|
|_Mr Smiths Scrapyard_|http://www.nexusmods.com/fallout3/mods/14075/|
|_NMCS Texture Pack_|http://www.nexusmods.com/fallout3/mods/12056/|
|_Personal Achievements Log_|http://www.nexusmods.com/fallout3/mods/11326/|
|_PipBoy 3000 HD Retexture_|http://www.nexusmods.com/fallout3/mods/20373/|
|_Project Reality_|http://www.nexusmods.com/fallout3/mods/17418/|
|_Pure Water_|http://www.nexusmods.com/fallout3/mods/2599/|
|_Realistic Death Physics_|http://www.nexusmods.com/fallout3/mods/12306/|
|_Retextured Clutter Collection_|http://www.nexusmods.com/fallout3/mods/6894/|
|_RH Ironsights_|http://www.nexusmods.com/fallout3/mods/6938/|
|_Rivet City Texture Pack_|http://www.nexusmods.com/fallout3/mods/3612/|
|_RobCo Certified Textures_|http://www.nexusmods.com/fallout3/mods/13428/|
|_RobCo Certified_|http://www.nexusmods.com/fallout3/mods/712/|
|_Robot Revolution HD - Protectron_|http://www.nexusmods.com/fallout3/mods/18902/|
|_SeraphTCs Personal Achievements Log FIX_|http://www.nexusmods.com/fallout3/mods/18678/|
|_Shiloh DS - Clean Pipboy Screen_|http://www.nexusmods.com/newvegas/mods/36255/|
|_SmoothLight - Pip-Boy Light Enhancer_|http://www.nexusmods.com/fallout3/mods/18389/|
|_The IMAGINATOR_|http://www.nexusmods.com/fallout3/mods/16875/|
|_The Institute - a fully voiced quest mod_|http://www.nexusmods.com/fallout3/mods/14449/|
|_To sleep - perchance to dream_|http://www.nexusmods.com/fallout3/mods/6921/|
|_UHQ Terrain Overhaul_|http://www.nexusmods.com/fallout3/mods/19799/|
|_Unofficial Fallout 3 Patch_|http://www.nexusmods.com/fallout3/mods/19122/|
|_User Interface Organizer_|http://www.nexusmods.com/fallout3/mods/20867/|
|_UWWUT - Unique Weapons With Unique Textures_|http://www.nexusmods.com/fallout3/mods/6309/|
|_Vault 101 Revisited_|http://www.nexusmods.com/fallout3/mods/13308/|
|_Weapon Mod Kits_|http://www.nexusmods.com/fallout3/mods/3388/|
|_Whats Your Brand - cigarette texture megapack_|http://www.nexusmods.com/fallout3/mods/591/|



### <a id="videos"></a>7.4. Videos

These are the videos which served as spiritual inspiration author of this guide. That's me.

* [Fallout 3 : To ENB or not to ENB](https://www.youtube.com/watch?v=BP3timf65O4) (21:36).
* [Fallout 3 Mod Clinic part 1 : Remastered, Blackened and Merged](https://www.youtube.com/watch?v=TeWV1wvg7cU) (24:12).
* [Fallout 3 Mod Clinic part 2 : RH Ironsights](https://www.youtube.com/watch?v=fHbJjkBSD4g) (16:33).
* [FALLOUT 3 Mod Clinic#3: UIO - User Interface Organizer](https://www.youtube.com/watch?v=bTlXOqV6pBA) (4:42).
* [Fallout 3 Multicore Crash Fix](https://www.youtube.com/watch?v=gIY2J6W8FBU) (03:17).
* [Fallout 3 Script Extender : FOSE (Installing and using)](https://www.youtube.com/watch?v=QK_f4vHiutA) (10:07).
* [Fallout New Vegas Mod Clinic #24 : UIO - User Interface Organizer](https://www.youtube.com/watch?v=qSA2BFQ2zc4) (11:23).
* [Load Order # 1 - What is it?](https://www.youtube.com/watch?v=YzsBKYUrcbE) (20:00).
* [Load Order # 2 - LOOT](https://www.youtube.com/watch?v=SzoyWugzZAw) (13:59).
* [Modding Fallout 3 - Part 1 : Getting Started with FWE and Marts Mutant Mod](https://www.youtube.com/watch?v=-SAeXsA6Nt8) (39:38).
* [Modding Fallout 3 - Part 2 : User Interface mods](https://www.youtube.com/watch?v=aqCzCXEydwU) (25:06).
* [Modding Fallout 3 - Part 3 : Weather and Lighting mods](https://www.youtube.com/watch?v=oHariRMIryI) (14:56).
* [Modding Fallout 3 - Part 4 : Performance & Stability (BASIC)](https://www.youtube.com/watch?v=tONiXNbwSt0) (26:38).
* [Modding Fallout 3 - Part 5 : Visual Enhancement mods](https://www.youtube.com/watch?v=ry-84eqDvr0) (30:00).
* [Modding Fallout 3 - Part 6 : Weapon Mod Kits (WMK) and EVE mods](https://www.youtube.com/watch?v=Vli2y7ZDUbo) (15:03).
* [Modding Fallout 3 - Part 7 : People Redesigned and Reanimated mods](https://www.youtube.com/watch?v=smLZNJIMCQA) (11:06).
* [Modding Fallout 3 - Part 8 : Unified HUD Project](https://www.youtube.com/watch?v=oSaJVzGmQaI) (11:00).
* [Modding Fallout 3 - Part 9 : FO3Edit](https://www.youtube.com/watch?v=uPK7R71zcwM) (39:13).
* [Skyrim Mod Tool TES5EDIT : Cleaning your master files (REVISED)](https://www.youtube.com/watch?v=fw3g_N1jcZQ) (13:24).
* [Fallout 3 mod : Advanced Recon Gear (Version 3.1)](https://www.youtube.com/watch?v=OsstmRso_Jw) (4:42).
* [Fallout 3 || Mod tutorial || Part 1: MMM, FWE & Blackened](https://www.youtube.com/watch?v=J4y4lui3l9U) (15:16).