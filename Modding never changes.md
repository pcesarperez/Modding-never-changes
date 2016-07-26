# Modding... Modding never changes




## Table of contents

* [1. Introduction](#introduction)
* [2. The tools we need](#toolsWeNeed)
* [3. Fixing the game](#fixingGame)
	* [3.1. Install the game](#installGame)
	* [3.2. Disable Games for Windows Live](#disableGFWL)
	* [3.3. Patching the game](#patchingGame)
	* [3.4. Cleaning up the master files](#cleaningMasterFiles)
	* [3.5. Enabling the console](#enablingConsole)
	* [3.6. Enabling access to 4+ GB of memory](#largeAddressAware)
	* [3.7. _Fallout 3_ Script Extender](#fose)
	* [3.8. Getting rid of stutter](#gettingRidStutter)
	* [3.9. Fake full-screen mode](#fakeFullScreen)
	* [3.10. Saving games the right way](#casm)
* [4. Enhancing the game](#enhancingGame)
	* [4.1. Improving the user interface](#improvingUserInterface)
		+ [4.1.1. Building the basement](#buildingBasement)
		+ [4.1.2. Face-washing the HUD](#faceWashingHUD)
		+ [4.1.3. Rearranging things](#rearrangingThings)
		+ [4.1.3. Seeing things just when you need to](#seeingThingsWhenNeeded)
		+ [4.1.4. Cleaning up your faithful companion](#retexturingPipBoy)
		+ [4.1.5. You don't want to ask for directions](#betterMap)
		+ [4.1.6. No more dots](#noMoreDots)
		+ [4.1.7. Shed some light here, please](#shedSomeLight)
	* [4.2. Lend me your ears](#lendMeYourEars)
	* [4.3. Playing the bad-ass way](#playingBadAss)
		+ [4.3.1. _Ad astra per aspera_](#adAstraPerAspera)
		+ [4.3.2. Fraternizing with the neighborhood](#fraternizingNeighborhood)
		+ [4.3.3. We need more firepower!](#weNeedMoreFirepower)
		+ [4.3.4. Expanding your world](#expandingYourWorld)
* [5. Resources](#resources)
	* [5.1. Tools](#tools)
	* [5.2. Guides](#guides)
	* [5.3. Mods](#mods)
	* [5.4. Videos](#videos)




## <a id="introduction"></a>1. Introduction

We, human beings, have a strange knack for imagining Doomsday. We like to depict our planet devastated by plagues, war (either biological or nuclear), alien attacks or all together at the same time.

One of the videogames that best shows how could be our world after a nuclear holocaust is _Fallout 3_. And [I'm not the only one](https://warisboring.com/why-fallout-is-the-best-nuclear-war-story-ever-told-5910918d28e4) with that feeling.

However, if you have been around the videogame scene for a while, you will know that _Fallout_ games can be completely enhanced using _mods_... Well, that is a complete understatement, as you could play a whole different game with the appropriate mods. Or you could break the game. That's the tricky part.

Getting right to the point, vanilla _Fallout 3_ sucks in many different ways. You cannot even run the game if your box uses Windows 7 or higher. A lot of tinkering has to be done for the game to run flawlessly.

There is an awesome [guide to fix the game in order to run under modern versions of Windows](http://steamcommunity.com/sharedfiles/filedetails/?id=149946772), written by [BenWah](http://steamcommunity.com/id/benwaa), which I intend to follow. And there are [a hell of a lot of videos by Gopher](https://www.youtube.com/channel/UC1CSCMwaDubQ4rcYCpX40Eg) with the best _Fallout 3_ mods your money can buy (well, sort of). Give credit when credit is due, you know.

So, there is no original work here, just an extended guide to put things into perspective. And this perspective is divided into two parts:

1. The firs part is about _fixing_ the game. At the end of this chapter, you will have a flawless _Fallout 3_ game, running smoothly, with no CTD (_Crash to Desktop_ in jargon), but it will be a vanilla game, at least content, graphics and audio-wise. No changes will be made to the story or the way you perceive the Wasteland.
2. The second part is about _enhancing_ the game. This is pretty based on personal taste, so feel free to ignore me (too bad) or, even better, modify this guide to your heart's content. I have picked the mods I like most, but your mileage may vary.

_I <del>don't</del> **DO** want to set the world on fire..._




## <a id="toolsWeNeed"></a>2. The tools we need

First and foremost, we need _Fallout 3 Game Of The Year Edition_ installed. This guide refers to the Steam version of the game.

We will need three additional tools to get the job done:

* [Nexus Mod Manager](http://www.nexusmods.com/games/mods/modmanager/?). This is the tool of choice when it comes to keep all your mods organized and up-to-date.
* [LOOT](https://loot.github.io/). Installing mods on Bethesda games can be a pain in the ass, especially if you try to install a lot of possibly-colliding mods. This tool keeps the load order straight.
* [FO3Edit](http://www.nexusmods.com/fallout3/mods/637/?). _Fallout 3_ itself comes out-of-the-box with certain errors in the main and DLC files, and this tool comes in handy to correct them. Besides, this is **THE** tool to create a merged patch to run the game with an absurd amount of mods.

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



### <a id="installGame"></a>3.1. Install the game

Pretty much straightforward, uh? Well, no. You need to run the game at least once to create the `.ini` files we will tinker with.

Again: you **MUST** run the game at least once in order to fix it.

The launcher dutifully informs you that video hardware is about to be detected, thus setting up the configuration for you.

![Fallout 3 video hardware detection](Images/Fallout%203%20video%20hardware%20detection.png)

Lucky me, my video card is up to the task (however, you don't want to know the specs of my box; no need to cry).

![High Quality settings set](Images/HQ%20settings%20set.png)

And here we go! This is the launcher in all its greenish glory.

![Fallout 3 launcher](Images/Fallout%203%20launcher.png)

Take a good look at it, for you are going to see this window **A LOT**. Trust me.

Finally, click on _Play_, and enjoy the view.

![Fallout 3 main menu](Images/Fallout%203%20main%20menu.png)

Bear in mind that no matter how hard you pray or curse, this is as far as the game gets running in any version of Windows higher than XP. But this is all we need, for now. Just click on _Quit_ and check this files and folders under `[%USERPROFILE%\Documents\My Games\Fallout3]`:

* `[Saves]`
* `FALLOUT3.INI`
* `FalloutPrefs.ini`
* `RendererInfo.txt`



### <a id="disableGFWL"></a>3.2. Disable Games for Windows Live

In BenWah's guide you can either update your Games for Windows Live (GFWL for short) installation, or disable it. Unless it's vital to you, I recommend disabling GFWL, just in case.

To disable GFWL, you need to download and run [Games for Windows LIVE disabler](http://www.nexusmods.com/fallout3/mods/1086/?).

**DON'T** use Nexus Mod Manager (NMM for short) to download this tool. Download it manually instead.

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

Thanks to the efforts of BenWah and other people around, we have the [Unofficial Fallout 3 Patch](http://www.nexusmods.com/fallout3/mods/19122/?), with a huge list of fixes and improvements.

Once downloaded (manually, not using NMM), just run the fairly large executable (over 200 MB) and follow the wizard:

1. Welcome window.
![UF3P Welcome window](Images/Unofficial%20Fallout%203%20Patch%201.png)
2. License agreement.
![UF3P License agreement](Images/Unofficial%20Fallout%203%20Patch%202.png)
3. Patch notes. These are important, as the clearly state that you should have the GOTY version of the game, with all DLC to take full advantage of the patch.
![UF3P Patch notes](Images/Unofficial%20Fallout%203%20Patch%203.png)
4. _Fallout 3_ location.
![UF3P Fallout 3 location](Images/Unofficial%20Fallout%203%20Patch%204.png)
5. Component selection. You should keep the default settings (all DLC and several minor but useful fixes).
![UF3P Component selection](Images/Unofficial%20Fallout%203%20Patch%205.png)
6. Start menu folder.
![UF3P Start menu folder](Images/Unofficial%20Fallout%203%20Patch%206.png)
7. Installation summary.
![UF3P Installation summary](Images/Unofficial%20Fallout%203%20Patch%207.png)
8. You should then see this window to be happy.
![UF3P Status check](Images/Unofficial%20Fallout%203%20Patch%208.png)
9. Here we go! It takes a while, because the patch moves around a lot of files.
![UF3P Installation progress](Images/Unofficial%20Fallout%203%20Patch%209.png)
10. When the installation finishes, the program shows a dialog with some techno-gibberish speak. Fear not! _Fallout 3_ [crashes if running in a box with multiple cores](http://www.sevenforums.com/gaming/20199-fallout-3-windows-7-w-quad-core.html), but the patch fixes the configuration options automatically. Click _Yes_, of course.
![UF3P Multicore fix](Images/Unofficial%20Fallout%203%20Patch%2010.png)
11. Happy ending!
![UF3P Happy ending](Images/Unofficial%20Fallout%203%20Patch%2011.png)

There is one final step to ensure that the patch is loaded in the proper place, at the bottom of the data files.

Each data file can come in two flavors: `.esm` for master files or `.esp` for secondary (patch) files. The DLCs themselves are `.esm` files.

This is a good time to check the load order of the game data files, so fire up LOOT to see what is happening under the hood. On a side note, Gopher has published two videos, one explaining [what is 'load order' and why it is important](https://www.youtube.com/watch?v=YzsBKYUrcbE) (20:00), and other explaining [what is LOOT and how to put it to good use](https://www.youtube.com/watch?v=SzoyWugzZAw) (13:59).

![LOOT first run after UF3P](Images/LOOT%20first%20run%20after%20UF3P.png)

After clicking on the leftmost icon, the program proposes the proper load order, meanwhile detecting data inconsistencies.

![LOOT after sorting](Images/LOOT%20after%20sorting.png)

You might be surprised to check that there are inconsistencies in the main DLC files, like `Anchorage.esm` (master file for _Operation Anchorage_ DLC). As we said, Bethesda is not known for releasing solid, fully tested programs. We'll address that later.

For now, just click on _Apply_ to put the unofficial patch at the bottom of the load order.

You should test the game right now. If everything went OK, you should be able to play the game.

![Fallout 3 first run](Images/Fallout%203%20first%20run.png)

Yippee ki-yay, motherfucker!



### <a id="cleaningMasterFiles"></a>3.4. Cleaning up the master files

Sure, you could play the game right now if you want. You would be playing a crippled, prone to crash game, but hey, if that's your thing...

We have miles to go before we sleep, though. Cheers for the brave who don't take second best!

As we saw earlier, the DLC data files themselves are somewhat _dirty_. This is what LOOT has to say about them:

* `Anchorage.esm`: Contains 54 ITM records and 10 deleted references.
* `ThePitt.esm`: Contains 40 ITM records and 5 deleted navmeshes.
* `BrokenSteel.esm`: Contains 275 ITM records, 34 deleted references and 12 deleted navmeshes.
* `PointLookout.esm`: Contains 21 ITM records.
* `Zeta.esm`: Contains 15 ITM records.

The only clean file in your load order is `Unofficial Fallout 3 Patch.esm`, as expected. No wonder, this is a huge patch that sits on the game and all its DLCs.

In every single case, LOOT has a sugestion: clean with [FO3Edit](http://www.nexusmods.com/fallout3/mods/637/?).

FO3Edit is an utility aimed at mod creators and users both, weighting more on the first group. Gopher has a fantastic video explaining [how to use TES5Edit (the _Skyrim_ version of the tool) to clean your master files](https://www.youtube.com/watch?v=fw3g_N1jcZQ) (13:24). You should left what you were doing right now and watch the video. I'll wait.

We are going to clean the master files, one by one. This guide about [cleaning files with TES5Edit](http://www.creationkit.com/index.php?title=TES5Edit_Cleaning_Guide_-_TES5Edit) comes in handy, but ignore it if you just want the heart of the issue.

I will show the instructions to clean one of the files, considering the rest are treated all the same.

1. Fire up FO3Edit. The tool does a good job detecting _Fallout 3_ data folder, thus showing all the data files we are using so far.
![FO3Edit master-plugin selection](Images/FO3Edit%20master-plugin%20selection.png)
2. Right-click on the floating window and select _Select none_. We are going to choose the files to clean, one by one.
![FO3Edit selecting none](Images/FO3Edit%20selecting%20none.png)
3. Now select the following files:
	* `Fallout3.esm`.
	* The data file you are going to clean (for example, `Anchorage.esm`).
![FO3Edit selecting files](Images/FO3Edit%20selecting%20files.png)
4. After a while, depending of the size of the data file, the tool finishes loading the data, plus the `Fallout3.exe` executable itself.
![FO3Edit file loaded](Images/FO3Edit%20file%20loaded.png)
5. Right-click on the `Anchorage.esm` node in the left panel tree and select _Apply filter for cleaning_.
![FO3Edit apply filter for cleaning](Images/FO3Edit%20apply%20filter%20for%20cleaning.png)
6. The filtering may take a little while, depending on how dirty the file is. When the filtering is completed, a line with the heading "[Filtering done]" appears in the right panel. The tree in the left panel shows the files with fancy colors which you don't have to give a fuck, unless you want to delve deeper into the inner workings of the mods.
![FO3Edit after filtering](Images/FO3Edit%20after%20filtering.png)
7. First, we are going to remove ITM (_Identical to Master_) records. They are not going to crash the game, but they take up space, and trust me, when you get the I-am-going-to-install-every-fancy-mod-available spree, you will need as much space as you can get. Right-click on the `Anchorage.esm` node in the left panel tree and select _Remove "Identical to Master" records_.
![FO3Edit remove ITM records](Images/FO3Edit%20remove%20ITM%20records.png)
8. Everytime you try to change a data file, a big warning appears. But, as seasoned hard-ass mod installers, we are sure as hell of what we are doing. Aren't we?
![FO3Edit warning](Images/FO3Edit%20warning.png)
9. After a little while, a message shows up in the right panel, reporting 43696 records processed and 54 records removed (don't worry if the numbers don't match; your setup may be slightly different).
![FO3Edit ITM records deleted](Images/FO3Edit%20ITM%20records%20deleted.png)
10. Next, we are going to undelete and disable deleted references... Unlike ITM records, which can be considered mostly harmless, deleted references can (and will) fuck up your game, because they are references to objects that _are supposed to be in the game_, but they no longer are, _and no one has marked them as disabled_. So, any mod using a deleted but not disabled reference is going to eventually crash your system. We are talking serious shit here. To get rid of these nasty sons of a bitch, right click on the `Anchorage.esm` node in the left panel tree and select _Undelete and Disable References_.
![FO3Edit undelete and disable references](Images/FO3Edit%20undelete%20and%20disable%20references.png)
11. A bit of processing again, and we have another message in the right panel, reporting 43642 records processed and 10 undeleted records.
![FO3Edit after undeleting and disabling](Images/FO3Edit%20after%20undeleting%20and%20disabling.png)
12. Job done! We just need to save the modified data file. To do that, just click on the close button of the tool window. A pop-up window should appear with _just one file_, the one you have been tinkering with (`Anchorage.esm`, in this case). If more than one file is shown, press <kbd>ESC</kbd> or click on the close button and start over again, because you surely screwed up at one point in the process. Anyway, make sure that the option _Backup plugins_ is selected before clicking _Ok_.
![FO3Edit save changed files](Images/FO3Edit%20save%20changed%20files.png)

You have to repeat the process for each and every one of the aforementioned data files.

In case you wonder, FO3Edit creates a folder named `[FO3Edit Backups]` under `[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data]` where it stores backup copies of the mods we have modified.

Run LOOT to be sure that we have a clean, patched game now.

![LOOT after cleaning](Images/LOOT%20after%20cleaning.png)

And, of course, run the game just to be on the safe side.

![Fallout 3 first patched run](Images/Fallout%203%20first%20patched%20run.png)

### <a id="enablingConsole"></a>3.5. Enabling the console

The game console is not strictly neccesary to fix the game, but it will come in handy to test the fixes we apply.

I am using the console to cheat my way out the Vault 101, because testing each new mod with a fresh start may be weary, to say the least.

Enabling the console means editing `FALLOUT3.INI` file in `[%USERPROFILE%\Documents\My Games\Fallout3]`, setting the following line, which should be enabled by default (make sure you make a backup copy first):

```INI
bAllowConsole=1
```

The actual key used to activate the console depends on the language layout you are using, but it should be to the left of the <kbd>1</kbd> key. In en-US keyboards it is bound to the tilde character <kbd>~</kbd>, but, for example, in the es-ES layout (Spanish), that key is bound to the numeral character <kbd>º</kbd>.

To test the console, start the game and press the corresponding key while in the main menu. A tiny vertical cursor will appear in the lower left corner of the screen. Run the following command:

```
GetDayOfWeek
```

The system should print something like:

```
GetDayOfWeek >> 5.00
```

![Fallout 3 testing the console](Images/Fallout%203%20testing%20the%20console.png)

There is no way to change the key assigned to the console, unless you install [_Console Key Binder_](http://www.nexusmods.com/fallout3/mods/2637/?) mod. However, you should keep your mod stack to a minimum. If you want to install this mod nonetheless, you should have installed first _Fallout Script Extender_, which we will be covering in [a later section](#fose).

Finally, there is an exhaustive [list of console commands](http://www.tweakguides.com/Fallout3_11.html) in the awesome [_Fallout 3 Tweaking Guide_](http://www.tweakguides.com/Fallout3_1.html).



### <a id="largeAddressAware"></a>3.6. Enabling access to 4+ GB of memory

_Fallout 3_ does not use all the available memory it could have due to its 32 bits nature. However, you can modify the game executable to take advantage of all the memory it can get.

Gopher explains the way to go with this video about [performance and stability in _Fallout 3_](https://www.youtube.com/watch?v=tONiXNbwSt0) (26:38) (the video touches several topics, but the one we are focusing on spans from the beginning to 08:55, give or take).

We don't want to clutter our system with unnecessary tools, so we are sticking with [Large Address Aware Enabler for _Fallout 3_](http://www.nexusmods.com/fallout3/mods/6510/?).

1. Download the mod manually (not using NMM), and extract its contents in a location of your choice (`[%LAA_FOLDER%]`, for reference).
2. Create a backup of the file `Fallout3.exe` from `[%STEAM_HOME%\steamapps\common\Fallout 3 goty]`.
3. Copy the file `Fallout3.exe` to `[%LAA_FOLDER]`.
4. Run `START.BAT` in `[%LAA_FOLDER%]`. A console window will appear, reporting that the patching is about to start. Press any key.
![LAA Enabler](Images/LAA%20Enabler%20reminder.png)
5. Several options are shown. We want to press <kbd>A</kbd> to add the LAA feature to _Fallout 3_ executable.
![LAA Enabler options](Images/LAA%20Enabler%20options.png)
6. LAA Enabler patches the executable and happily informs us about it. Press any key.
![LAA Enabler successful](Images/LAA%20Enabler%20successful.png)
7. The program goes back to the options window. Press <kbd>E</kbd> to exit.
8. Copy back `Fallout3.exe` to its original location.

And that's really it. Now _Fallout 3_ is prepared to handle more than 2 GB of RAM, improving stability.



### <a id="fose"></a>3.7. _Fallout 3_ Script Extender

If you ever want to install a single mod in _Fallout 3_, you will need [_Fallout Script Extender_](http://fose.silverlock.org/) (FOSE, for short).

Well... That's not exactly true, as there may be mods that does not make use of the capabilites provided by FOSE (we have been using a few, so far). But they will be a minority. And we will need this tool ahead the road.

As usual, Gopher has published a worth watching video about the [installation and use of FOSE](https://www.youtube.com/watch?v=QK_f4vHiutA) (10:07).

1. Download the latest version of FOSE ([1.2b2](http://fose.silverlock.org/download/fose_v1_2_beta2.7z) as of this writing). You should download the 7Z version (not the loader).
2. Extract the contents of the archive into a folder of your choice.
3. Copy the contents of the folder to `[%STEAM_HOME%\steamapps\common\Fallout 3 goty]`, except the folder `[src]`, which contains FOSE source code.
4. Create a shortcut for the file `fose_loader.exe` in a location of your choice (e.g., your desktop).
5. Rename the shortcut to whatever name you feel comfortable with. I go with _Fallout 3_, because I keep the older shortcut, using the launcher, to configure the game, thus renaming it to _Fallout 3 (config)_.
![Fallout 3 launch shortcuts](Images/Fallout%203%20launch%20shortcuts.png)
6. If you, like me, think that the default shortcut icon is [Deathclaw](http://fallout.wikia.com/wiki/Deathclaw) shit, it might be worth considering an [alternate icon](http://www.iconarchive.com/show/mega-games-pack-23-icons-by-3xhumed/Fallout-3-new-1-icon.html). Download the `.ico` version and copy it to `[%STEAM_HOME%\steamapps\common\Fallout 3 goty]`.
7. Right-click on the shortcut icon and select _Properties_.
![Fallout 3 shortcut properties](Images/Fallout%203%20shortcut%20properties.png)
8. In the _Shortcut_ tab, select the option _Change icon..._.
![Fallout 3 shortcut change icon](Images/Fallout%203%20shortcut%20change%20icon.png)
9. The system dutifully informs you that `fose_loader.exe` (the executable the shortcut refers to) does not contain any available icon. Click _Ok_.
![Fallout 3 shortcut no default icon](Images/Fallout%203%20shortcut%20no%20default%20icon.png)
10. The system shows a floating window where you could select one of the shitty system default icons. Just click on _Browse_...
![Fallout 3 shortcut select icon](Images/Fallout%203%20shortcut%20select%20icon.png)
11. Select the `.ico` file you downloaded before and click _Open_.
![Fallout 3 shortcut open icon](Images/Fallout%203%20shortcut%20open%20icon.png)
12. Back to the icon selection window, click on _Ok_.
![Fallout 3 shortcut icon selected](Images/Fallout%203%20shortcut%20icon%20selected.png)
13. Back to the properties window, click on _Ok_.
![Fallout 3 shortcut properties final](Images/Fallout%203%20shortcut%20properties%20final.png)
14. _Et voila!_ We have now two great-looking icons to launch _Fallout 3_, one to configure it and the other to actually launch a mod-friendly version of the game.
![Fallout 3 launch shortcuts final](Images/Fallout%203%20launch%20shortcuts%20final.png)
15. We are going to test that FOSE is correctly installed, and for that, launch the game with the new shortcut. In the main menu screen, activate the console and write `GetFOSEVersion`. You should get something like `FOSE version: 1`.
![Fallout 3 FOSE installed](Images/Fallout%203%20FOSE%20installed.png)

FOSE provides a [whole new set of console commands](http://fose.silverlock.org/fose_command_doc.html) you can use, although they are not strictly necessary.



### <a id="gettingRidStutter"></a>3.8. Getting rid of stutter

_Fallout 3_ suffers from stuttering, this is, there are certain points in the game where the visuals are lacking in fluidity. Although this can be reduced by optimizing your system (updating your graphics driver to the top, unfragmenting the hard drive, and so on), there is still a micro-stuttering that can be perceived in lower-spec machines when framerate suddenly changes.

In the same video about [performance and stability](https://www.youtube.com/watch?v=tONiXNbwSt0) (26:38), Gopher talks about this problem, from minute 08:55 to 16:40, more or less. We are going to install our first mod (apart from the unofficial patch), and for this, we are going to need [_Nexus Mod Manager_] or NMM. This is the tool that allows to keep track of the installed mods, along with their updates.

Provided that you have installed NMM:

1. Run NMM. If this is the first time you do so, NMM searchs for the games it knows of, modding-wise. In this context, we are only interested in _Fallout 3_, so as soon as NMM finds it, we should confirm the location (with the green tick mark under the name of the game) and then clicking on _Ok_.
![NMM searching for games](Images/NMM%20searching%20for%20games.png)
2. NMM shows then a game selection window, with a list of games which mods NMM is managing. Select _Fallout 3_ and click on _Ok_ (you can select _Don't ask me next time_, if you feel like to).
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
8. Open [_Fallout Stutter Remover_](http://www.nexusmods.com/fallout3/mods/8886/?) mod page in your browser and navigate to the _Files_ tab. We need the latest version (4.1.36 as of this writing) and nothing else. Download this with the manager. The mod is fairly small, so it takes a breeze to download. When downloaded, you should see something like this in NMM (adjust the user interface as necessary).
![NMM FSR downloaded](Images/NMM%20FSR%20downloaded.png)
9. Select the FSR mod in the main panel, and click on the big green check mark on the left button bar to install it.
![NMM select FSR to install](Images/NMM%20select%20FSR%20to%20install.png)
10. Now, you should see a little green check mark to the left of the name of the mod, along with a message in the _Mod Activation Queue_ panel reporting that the installation is complete.
![NMM FSR installation](Images/NMM%20FSR%20installation%20complete.png)
11. Edit the file `sr_Fallout_Stutter_Remover.ini` in `[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data\FOSE\Plugins]` and change the value of the `bInject_iFPSClamp` to 1. Save the file and we are good to go!



### <a id="fakeFullScreen"></a>3.9. Fake full-screen mode

Believe or not, one of the things that could produce a CTD every other game, is the full-screen mode. As usual, Gopher has a [video explaining the problem](https://www.youtube.com/watch?v=tONiXNbwSt0) (26:38), same as before (this part spans roughly from 17:30 to the end).

1. Download manually the [_Fake Fullscreen Mode Windowed_](http://www.nexusmods.com/fallout3/mods/16001/?) mod, not with NMM.
2. Extract the contents of the downloaded archive to a location of your choice.
3. Inside that folder there should be just one file, `Fallout_Fullscreen.exe`. Copy the file to `[%STEAM_HOME%\steamapps\common\Fallout 3 goty]`.
4. Create a shortcut to `Fallout_Fullscreen.exe` wherever you want, and rename it to _Fallout 3 (fullscreen)_, for example.
![Fallout 3 launch shortcuts with fullscreen](Images/Fallout%203%20launch%20shortcuts%20with%20fullscreen.png)
5. Run the launcher (_Fallout 3 (config)_, remember?), and select _Options_. Take note of your current resolution.
![Fallout 3 options](Images/Fallout%203%20options.png)
6. Mark _Windowed mode_ and change the resolution to the previous one (every time you change to windowed mode and back, the resolution combo resets). Click _Ok_ and exit the launcher.
![Fallout 3 options windowed](Images/Fallout%203%20options%20windowed.png)
7. Run the game with the new shortcut. The game will start with the window border, but after a little while, the window border disappears, resembling the actual fullscreen mode. This version is fully compatible with FOSE, which you can test running `GetFOSEVersion` in the console.



### <a id="casm"></a>3.10. Saving games the right way

The sun rises in the East, Michael Fassbender is better than you in everything and _Fallout 3_ crashes. You need to come to terms with these simple truths of life.

Even with a fully patched game, _Fallout 3_ spits you out to the desktop now and then. In these cases, your only way back is to restore a saved game. But saved games do get corrupted sometimes. And, unless you have been saving your game **A FUCKING LOT**, and when I say "saving", I mean _not quicksaving_, you are doomed.

There is a mod called [CASM](http://www.nexusmods.com/fallout3/mods/3729/?) to address that problem. CASM automates saving your game in a sensible way, and it provides two key shortcuts to replace the standard quicksave/quickload built-in feature:

* <kbd>F4</kbd> replaces <kbd>F5</kbd>, creating a _named_ saved game.
* <kbd>F8</kbd> replaces <kbd>F9</kbd>, loading the last saved game.

CASM also saves the game automatically with a given frequency and under certain events. Let's see how to install this mod.

1. Launch the game. When the main menu appears, click on _Settings_ and then _Gameplay_.
![Fallout 3 gameplay settings](Images/Fallout%203%20gameplay%20settings.png)
2. Disable all three options (_Save On Rest_, _Save On Wait_ and _Save On Travel_).
![Fallout 3 autosave disabled](Images/Fallout%203%20autosave%20disabled.png)
3. Exit the game and download CASM using NMM.
![NMM CASM downloaded](Images/NMM%20CASM%20downloaded.png)
4. Activate CASM double-clicking on the mod name.
![NMM CASM installation complete](Images/NMM%20CASM%20installation%20complete.png)
5. Check that CASM is loaded at the bottom of the mod stack in the _Plugins_ tab of NMM.
![NMM CASM loaded last](Images/NMM%20CASM%20loaded%20last.png)
6. Close NMM and run LOOT. Click on the _Sort Plugins_ icon to fix the load order. Notice that CASM still sits at the bottom, and no conflicts are detected (this step is fairly unnecessary, but you need to get used to routinely rearrange your load order).
![LOOT after installing CASM](Images/LOOT%20after%20installing%20CASM.png)
7. CASM is configurable through an in-game option in your Pip-Boy 3000 (you will get your own Pip-Boy at the age of 10). Fire up your Pip-Boy by pressing <kbd>TAB</kbd> and navigate to the _Aid_ section. You will see an "item" called _CASM Options Menu_.
![Fallout 3 CASM option](Images/Fallout%203%20CASM%20option.png)
8. Click on the CASM item _and then exit the Pip-Boy_ by pressing again <kbd>TAB</kbd> (yeah, not the most intuitive thing in the world). A screen with CASM settings is shown. There are a lot of options for you to configure, although the default settings are pretty good to go.
![Fallout 3 CASM settings](Images/Fallout%203%20CASM%20settings.png)




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

First things first, we are going to need a way for all the mods to collaborate seamlessly, and for this, we are going to install [_User Interface Organizer_](http://www.nexusmods.com/fallout3/mods/20867/?), or UIO. This mod will keep every important user interface mod out there in line.

If you have followed the guide so far, you have a grasp of the basics to download, activate and reorder any mod, so:

1. Download UIO with NMM.
2. Activate it.

And that's really it. No need to use LOOT because this is a FOSE plugin. FOSE plugins are placed in `[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data\FOSE\Plugins]`, so there should be a file named `ui_organizer.dll` in that folder.


#### <a id="faceWashingHUD"></a>4.1.2. Face-washing the HUD

Next, we are going to _shrink_ the user interface using [_DarNified UI F3_](http://forums.bethsoft.com/topic/1121454-wipzbeta-darnified-ui-f3/), or DUIF3.

This will be a bit tricky, because there are no NMM packages right out-of-the-box. Instead, we have the FOMOD ([_Fallout Mod Manager_](http://www.nexusmods.com/fallout3/mods/640/?)) packages... But they are compatible with NMM, so bear with me.

1. Download [DUIF3 Alpha<sup>11</sup>](http://ui.darnified.net/wip/F3/dui_f3a11.zip).
2. Download [DUIF3 Alpha<sup>11</sup> Hotfix](http://ui.darnified.net/wip/F3/dui_f3a11_HF.7z).
3. Start NMM, go to the _Mods_ tab and click on the green plus sign to add mod from file.
![NMM Adding mod from file](Images/NMM%20Adding%20mod%20from%20file.png)
4. In the file selector that appears, navigate to the location of the downloaded DUIF3 files and open `dui_f3a11.zip`, corresponding to the main file.
5. Repeat the process for the patch, `dui_f3a11_HF.7z`.
![NMM DUIF3 files loaded](Images/NMM%20DUIF3%20files%20loaded.png)
6. The mods have no very friendly names, but we can change it in NMM. Just click on the main mod (DarNified UI F3 alpha) and click on the _Gets missing mod info_ icon.
![NMM change DUIF3 mod name](Images/NMM%20change%20DUIF3%20mod%20name.png)
7. In the window with the mod info, change the contents of the _Name_ field to "DarNified UI F3 Alpha 11" and click _Ok_.
![NMM edit mod information](Images/NMM%20edit%20mod%20information.png)
8. Do the same for the hotfix, renaming it to "DarNified UI F3 Alpha 11 Hotfix". Check the new names in NMM.
![NMM DUIF3 friendly names](Images/NMM%20DUIF3%20friendly%20names.png)
9. Activate the main mod file by double-clicking on it. Eventually, you will be asked to confirm if you want to use the fonts provided with DUIF3. As crazy as it sounds, you want to say _No_, for now.
![NMM DUIF3 font config confirmation](Images/NMM%20DUIF3%20font%20config%20confirmation.png)
10. Activate the hotfix and answer _Yes to all_ when asked to overwrite previous files (from the main mod file, in fact).
![NMM DUIF3 hotfix overwriting](Images/NMM%20DUIF3%20hotfix%20overwriting.png)
11. Check that DUIF3 is installed in the _Plugins_ tab.
![NMM DUIF3 installed](Images/NMM%20DUIF3%20installed.png)
12. Just in case, use LOOT to sort your load order session. It is not really necessary, as DUIF3 sits on the bottom, but you need to flex your muscles now and then.
![LOOT DUIF3](Images/LOOT%20DUIF3.png)
13. Remember when we said "no" to use the fonts provided by DUIF3? There is an error in NMM, possibly related to modifying files in certain protected Windows folders, which crashes the program. So, go back to the [DUIF3 page](http://forums.bethsoft.com/topic/1121454-wipzbeta-darnified-ui-f3/) and copy the text block starting with `[Fonts]`. I have even made half the job for you.
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
14. Open the file `FALLOUT.INI` in `[%USERPROFILE%\Documents\My Games\Fallout3]` and paste the text over the `[Fonts]` section.
15. Launch the game and check the Vault-boy head in the lower-left corner of the screen. If you hover with the mouse over the head, you will see something like that (version numbers may vary):
```
Fallout 3 1.7.0.3
DarNified UI F3 0.11.1a
Powered by FOSE 1.2 b2
```
16. As a collateral effect, _LIVE_ button in the main screen is enabled again, but fear not! This is nothing but DUIF3 taking full control of your interface settings in a somewhat standard way. GFWL is still disabled.
![Fallout 3 DUIF3 installed](Images/Fallout%203%20DUIF3%20installed.png)
17. Start a new game or continue a previous one, and check the smaller HUD elements, including new information about date and time in the upper-right corner of the screen.
![Fallout 3 DUIF3 small HUD](Images/Fallout%203%20DUIF3%20small%20HUD.png)
18. If you press <kbd>ESC</kbd> in game, you will see a new option at the right to configure DUIF3.
![Fallout 3 DUIF3 ingame option](Images/Fallout%203%20DUIF3%20ingame%20option.png)
19. There are a lot of settings for you to configure, adjusting the HUD to your liking.
![Fallout 3 DUIF3 settings](Images/Fallout%203%20DUIF3%20settings.png)


#### <a id="rearrangingThings"></a>4.1.3. Rearranging things

For those of you who don't like the default layout of the Heads Up Display (HUD), there is a little mod (little in size, that is) which helps you to change exactly that: [_Adjustable HUD_](http://www.nexusmods.com/fallout3/mods/15886/?) or aHUD.

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
	* `aHUD.esm`
	* `CASM.esp`
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

In addition to have the HUD elements placed where you like, you can improve the immersion by hiding these elements when you don't need them. I like to have them hidden when I am wandering around and have them shown when I am in combat. We have [_Immersive HUD_](http://www.nexusmods.com/fallout3/mods/15790/?) or iHUD for this.

1. Download the mod with NMM.
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
	* `iHUD.esm`
	* `CASM.esp`
	* `DarNifiedUIF3.esp`
5. Launch the game and notice the absence of HUD elements on screen.
![Fallout 3 iHUD default](Images/Fallout%203%20iHUD%20default.png)
6. keep key <kbd>I</kbd> pressed a few moments. The iHUD settings menu will appear.
![Fallout 3 iHUD settings](Images/Fallout%203%20iHUD%20settings.png)
7. There are a lot of customization options in iHUD. Tweak around until you feel comfortable with the results ([Gopher's video](https://youtu.be/aqCzCXEydwU?t=18m20s) should help, around 18:20).


#### <a id="retexturingPipBoy"></a>4.1.4. Cleaning up your faithful companion

One of the things you are going to see a lot in this game is your Pip-Boy. And when I say "a lot", I mean an awful-fucking lot. It's your personal assistant, after all.

It's a little sad to see that glorious piece of junk in low resolution, so, let's improve how it looks, using [_PipBoy 3000 HD Retexture_](http://www.nexusmods.com/fallout3/mods/20373/?).

1. Download and activate the mod using NMM. There shouldn't be any overwritten files.
2. This is a pure textures mod, so there are no `.esm` or `.esp` files here. No need to LOOT-reorder your files then.
3. Launch the game and just compare.

Before:
![Fallout 3 Pip-Boy before retexturing](Images/Fallout%203%20Pip-Boy%20before%20retexturing.png)

After:
![Fallout 3 Pip-Boy after retexturing](Images/Fallout%203%20Pip-Boy%20after%20retexturing.png)


#### <a id="betterMap"></a>4.1.5. You don't want to ask for directions

Let's face it: the vanilla map in _Fallout 3_ seems to have been produced from Dora the explorer's backpack. And you don't want to start asking directions in D.C., because super-mutants are not known for their kindness of heart with strangers.

We are going to use [_Better High Detail Map and Icons_](http://www.nexusmods.com/fallout3/mods/16898/?) to have decent maps.

1. Download and activate the mod with NMM. It will take a while, because the texture files are pretty big (43 MB or so).
2. NMM shows a floating window with the installation options for the mod. Choose one map size and brightness (I chose 8k with roads and 50% more brightness, but your mileage may vary). Click on _Next_.
![NMM Better High Detail Map and Icons install options](Images/NMM%20Better%20High%20Detail%20Map%20and%20Icons%20install%20options.png)
3. Next window contains the customization options for the mod. I checked "Custom icons", "Clean Pipboy Screen" and green markers. Click on _Finish_.
![NMM Better High Detail Map and Icons customization options](Images/NMM%20Better%20High%20Detail%20Map%20and%20Icons%20customization%20options.png)
4. Answer _Yes to all_ when asked to overwrite files.
5. Launch the game, fire up your Pip-Boy and compare.

Before:

![Fallout 3 world map before](Images/Fallout%203%20world%20map%20before.png)

After:

![Fallout 3 world map after](Images/Fallout%203%20world%20map%20after.png)

There's just a single caveat: the hot click area for the options in the _Data_ section of your Pip-Boy gets shrinked to a few pixels below each option:

Outside the hot click area:

![Fallout 3 data option outside hot zone](Images/Fallout%203%20data%20option%20outside%20hot%20zone.png)

Inside the hot click area:

![Fallout 3 data option inside hot zone](Images/Fallout%203%20data%20option%20inside%20hot%20zone.png)

If you feel uncomfortable with this, open the file `map_menu.xml` in `[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data\Menus\main]` and change the values of the `<height />` tags for these three elements:

1. Around line 149:
```XML
<hotrect name="MM_LocalMap_ClipWindow">
	...
	<height> 660 </height>
	...
</hotrect>
```
2. Around line 268:
```XML
<hotrect name="MM_WorldMap_ClipWindow">
	...
	<height> 660 </height>
	...
</hotrect>
```
3. Around line 393:
```XML
<hotrect name="MM_Highlight_ClipWindow">
	...
	<height> 660 </height>
	...
</hotrect>
```

Just lower the value between 5 and 20 pixels, using the same value in the three elements. Notice the increment in the clickable zone using a value of 640 pixels at expense of map height.

![Fallout 3 data option hot zone expanded](Images/Fallout%203%20data%20option%20hot%20zone%20expanded.png)


####<a id="noMoreDots"></a>4.1.6. No more dots

There's one final thing left to have a perfect-although-cranky GPS in our hands (literallly). Have you noticed the small white dots in your map connecting where you are and your current quest location?

![Fallout 3 white dots](Images/Fallout%203%20white%20dots.png)

Well, in mathematics the straight line may be the shortest path between two points, but in real life, and specially in the Capital Wasteland, it usually is the shortest path between you and a Darwin-cleansing-style death. So, let's remove the goddamn dots with [_No more dots_](http://www.nexusmods.com/fallout3/mods/15918/?).

1. Download the mod with NMM.
2. Activate it by double-clicking.
3. That's it.

There's no `.esp` or `.esm` installed with this mod, so there's no need to rearrange the load order. Just launch the game and check your map.

![Fallout 3 no more dots](Images/Fallout%203%20no%20more%20dots.png)


####<a id="shedSomeLight"></a>4.1.7. Shed some light here, please

Lighting in _Fallout 3_ is somewhat weird. Sometimes you will find your self into what seems to be a lucid LSD-induced dream, with overexposed lights all around you. If you use your Pip-Boy's lamplight, things get much worse.

This small mod, [_SmoothLight - Pip-Boy Light Enhancer_](http://www.nexusmods.com/fallout3/mods/18389/?), comes to the rescue. Here we go.

1. Download and activate the mod with NMM. There souldn't be any conflicts.
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
	* `DarNifiedUIF3.esp`
	* `HZSmoothLight - FO3.esp`
3. Launch the game and activate your Pip-Boy's lamplight long-pressing the <kbd>TAB</kbd> key in a dark area.

See the difference for yourself.

With no light:

![Fallout 3 no Pip-Boy light](Images/Fallout%203%20no%20Pip-Boy%20light.png)

With standard light:

![Fallout 3 standard light](Images/Fallout%203%20standard%20light.png)

With enhanced light:

![Fallout 3 enhanced light](Images/Fallout%203%20enhanced%20light.png)

The difference is subtle, more noticeable in dark interiors.



###<a id="lendMeYourEars"></a>4.2. Lend me your ears

One of the most underrated things in videogames is audio. Every gamer out there crave for the ultimate graphics experience when playing her now-favorite-videogame. But audio is a subtle but very important part of that experience. Good ambient sounds and soundtrack can make your journey something memorable.

There is just one mod in this chapter, [_Fallout 3 - HD Audio Overhaul - v1.21_](http://www.nexusmods.com/fallout3/mods/13055/?), and it's a complete overhaul of all things related with audio in _Fallout 3_, from ambient sounds to soundtrack.

This mod is _massive_, so grab a mug of coffee and stay tuned with the latest news while installing it. You just have to download and install it with NMM. No conflicts should arise.

Launch the game and _listen_ carefully...



###<a id="playingBadAss"></a>4.3. Playing the bad-ass way

We have a pretty much vanilla game up to this point. Yeah, we changed the way the game looks in the previous chapter, but the base game still remains the same.

We are going to dramatically change that. Think of a chicken nugget that turns itself into a _filet mignon_, all of a sudden.

I would recommend creating a backup of your game, even though It will rack up to 7 GB of space or more. Better safe than starting the process all over again... And trust me, I know what I am talking about.


#### <a id="adAstraPerAspera"></a>4.3.1. _Ad astra per aspera_

The title of this chapter means "through hardships to the stars", in Latin, and it would be a good way to define our next mod: [_Fallout 3 Wanderers Edition_](http://www.nexusmods.com/fallout3/mods/2761/?), or FWE. As usual, Gopher has a video [explaining how to install FWE](https://www.youtube.com/watch?v=-SAeXsA6Nt8), and there is a [page for the project](https://sites.google.com/site/fo3wanderersedition) with lots of useful information.

The list of changes made by FWE is so long and their implications so deep that you'd better read the mod page to get a glimpse of that. The bottom line is: you will be playing a harsher, more challenging version of the game.

We will be needing five files:

* FWE Master Release 6-0 - Part 1.
* FWE Master Release 6-0 - Part 2.
* FWE 6-03a HOTFIX PATCH.
* DarnUI Support for FWE 6-02
* Immersive HUD - iHUD - Immersive HUD - Darnified FWE Patch

The last one can be downloaded from [the iHUD page](http://www.nexusmods.com/fallout3/mods/15790/?).

1. Download all the files with NMM, but _do not activate them_.
![NMM FWE entries](Images/NMM%20FWE%20entries.png)
2. Double click on _FWE - FO3 Wanderers Edition_ to bring up a window with some options. Leave all default options checked and check _Alternate Travel_, and maybe [_VATS Halftime_ and _VATS Realtime_](https://sites.google.com/site/fo3wanderersedition/detailed-changes/02combat#TOC-VATS-Tweaks) if you feel up to.
![NMM FWE setup](Images/NMM%20FWE%20setup.png)
3. The installation takes a while, for the mod is _huge_...
![NMM FWE installing](Images/NMM%20FWE%20installing.png)
4. Finally, the manager notifies us about a successful installation.
![NMM FWE installed](Images/NMM%20FWE%20installed.png)
5. Double click on _FWE - FO3 Wanderers Edition - Part 2 Assets_ to install the second part of the mod. This time, the mod gets installed silently.
![NMM FWE two files installed](Images/NMM%20FWE%20two%20files%20installed.png)
6. Double click on _FWE - FO3 Wanderers Edition - 6.03 HOTFIX_, and just accept the overwriting of some files in the main mod.
![NMM FWE confirm hotfix overwrite](Images/NMM%20FWE%20confirm%20hotfix%20overwrite.png)
7. Now check the _Plugins_ tab. There are two uninvited guests there: the two `.esp` files corresponding to options we did not choose to install (_Optional Restore Tracers_ and _Optional Restore Tracers (automatics only)_).
![NMM FWE uninvited guests](Images/NMM%20FWE%20uninvited%20guests.png)
8. We don't want any unwanted mod cluttering our load order, so let's navigate to the folder where mod files are installed (`[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data]`), and just delete the two offending `.esp` files.
![NMM FWE deleting unwanted files](Images/NMM%20FWE%20deleting%20unwanted%20files.png)
9. Relaunch NMM and check the files are vanished.
![NMM FWE plugins](Images/NMM%20FWE%20plugins.png)
10. Double click on _FWE - FO3 Wanderers Edition - DarnUI Support for FWE 6-02_ and answer _Yes to all_ when asked to overwrite files.
11. Double click on _Immersive HUD - iHUD - Immersive HUD - Darnified FWE Patch_ and answer _Yes to all_ when asked to overwrite files.
12. A number of files has been installed, so we need to rearrange our load order. Fire up LOOT and sort the files. This should be your load order:
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
	* `CASM.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `DarNifiedUIF3.esp`
13. LOOT warns you that certain files are somewhat dirty, so a cleaning with FO3Edit is in order. Just clean the files following the same steps we did in [the chapter about cleaning up the master files](#cleaningMasterFiles). To clean each file, select just this file in FO3Edit and let the tool select the set of files it depends on. For example, if you select `FO3 Wanderers Edition - Main File.esm`, the following files will be loaded altogether:
	* `Fallout3.esm`
	* `Fallout3.exe`
	* `CRAFT.esm`
	* `CALIBR.esm`
14. When all the files have been cleaned, run LOOT again and check there are no ITM records or undeleted references in your load order. There shouldn't be any.
15. And that's it. We have FWE completely installed. Launch the game and start a new game (yes, a new game). At certain point, you may choose between the classic storyline or an alternate start.
![Fallout 3 FWE alternate start](Images/Fallout%203%20FWE%20alternate%20start.png)
16. You can assign your skills, perks and even a background story in a terminal right in front of you right after waking up.
![Fallout 3 FWE special terminal](Images/Fallout%203%20FWE%20special%20terminal.png)
17. When you have selected the skill set for your journey, just sleep in the mat on the floor and wake up to your new life. After a moment, a dialog will appear talking about _Wasteland Explorer_, a motorcycle which replaces fast travel (we disabled it, remember?). Enable it for good.
![Fallout 3 FWE Wasteland Explorer enabled](Images/Fallout%203%20FWE%20Wasteland%20Explorer%20enabled.png)
18. And now we are at it... Remember when we relocated the HUD elements to fit our needs? Well, FWE resets that, so, regrettably, you will have to relocate them again.
![Fallout 3 FWE HUD reset](Images/Fallout%203%20FWE%20HUD%20reset.png)
19. Pull out your Pip-Boy and go to the _Items_ and then _Apparel_. There it is the option to configure FWE.
![Fallout 3 FWE Pip-Boy option](Images/Fallout%203%20FWE%20Pip-Boy%20option.png)
20. Click on the option to show the shitload of configurable settings for this mod.
![Fallout 3 FWE settings](Images/Fallout%203%20FWE%20settings.png)

You may be wondering why the hell we installed aHUD first and then FWE... Well, it's a matter of scalability. Each chapter in the enhancing section will give you a playable milestone. The first one was about having an improved UI, and this one is about playing a radically different game. Each section builds on top of the previous one, but, in this case, the drawbacks are no big deal.

From this point on, we will be using [_The Mergers_](http://www.nexusmods.com/fallout3/mods/16787/?), from Paradox Ignition. These are merged patches for the main mods we are going to install. They are aimed to reduce the file load in our data folder and increase stability.


#### <a id="fraternizingNeighborhood"></a> 4.3.2. Fraternizing with the neighborhood

If you like real challenges, you will **love** [_Martigen's Mutant Mod_](http://www.nexusmods.com/fallout3/mods/3211/?), or MMM, for short. MMM adds a lot of color to the game, in the form of new (and tougher) enemies, increased spawn rates, and so on.You will have plenty of rotten flesh-shaped love.

1. Download the files _Marts Mutant Mod 1-RC61 FOMOD Ready_ and _MMM-6_2-update_ with NMM (yeah, half of this book is plagued with acronyms; I am acutely aware of that).
2. Download _Marts Mutant Mod Merged_ from [_The Mergers_](http://www.nexusmods.com/fallout3/mods/16787/?) page with NMM. Notice the downloaded files.
![NMM MMM files downloaded](Images/NMM%20MMM%20files%20downloaded.png)
3. Activate _Martigen's Mutant Mod_ by double-clicking on it. NMM shows a window to select the preferred configuration method. We will choose the in-game menu, as it requires far less tinkering than its ESP counterpart.
![NMM MMM menu configuration](Images/NMM%20MMM%20menu%20configuration.png)
4. In the next window, all the DLC options should be checked, but leave the global options unchecked. More on that later.
![NMM MMM global options](Images/NMM%20MMM%20global%20options.png)
5. MMM overwrites several files from FWE, as it overhauls the monster system in the game. Let it do its magic.
![NMM MMM FWE overwrite](Images/NMM%20MMM%20FWE%20overwrite.png)
6. Activate the RC6.2 update in NMM, overwriting any file from MMM original installation.
7. There are certain files we don't need in our setup, so close NMM and browse to the _Fallout 3_ data folder (`[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data]`). Delete the following files:
	* `Mart's Mutant Mod - Natural Selection.esp`
	* `Mart's Mutant Mod - Tougher Traders.esp`
	* `Mart's Mutant Mod - Zones Respawn.esp`
8. We are going to get rid of the files instaled by MMM to use the merged path we downloaded before. Create a folder in your data folder (namely `[MMM backup]`), and move the following files:
	* `Mart's Mutant Mod.esm`
	* `Mart's Mutant Mod.esp`
	* `Mart's Mutant Mod - DLC Anchorage.esp`
	* `Mart's Mutant Mod - DLC The Pitt.esp`
	* `Mart's Mutant Mod - DLC Broken Steel.esp`
	* `Mart's Mutant Mod - DLC Point Lookout.esp`
	* `Mart's Mutant Mod - DLC Zeta.esp`
	* `Mart's Mutant Mod - Master Menu Module.esp`
9. Reopen NMM and activate _Paradox Ignition presents The Mergers - Marts Mutant Mod Merged_ in the _Mods_ tab. The merged patch will ask for permission to overwrite already installed files. Proceed as usual.
![NMM MMM merged patch overwriting](Images/NMM%20MMM%20merged%20patch%20overwriting.png)
10. In the _Plugins_ tab, check the presence of the file `Mart's Mutant Mod.esm`, replacing all the files we installed before.
![NMM MMM installed](Images/NMM%20MMM%20installed.png)
11. Run LOOT as usual and rearrange your load order. This should be the deal:
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
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `Mart's Mutant Mod.esm`
	* `CASM.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `DarNifiedUIF3.esp`
12. Launch the game and pull up your Pip-Boy. Navigate to the _Items_ button, _Apparel_ section, where you will see a new entry called _MMM Control Panel_.
![Fallout 3 MMM control panel option](Images/Fallout%203%20MMM%20control%20panel%20option.png)
13. Click on the aforementioned option and wade through the zillions of options to fine-tune your monster-hunting experience.
![Fallout 3 MMM settings](Images/Fallout%203%20MMM%20settings.png)

Take into account that we need a [_Blackened_ compatibility patch](http://www.nexusmods.com/fallout3/mods/18173/?) to run FWE and MMM seamlessly, but these patches come in combos, so we are going to use the one which suits best our mod stack.


#### <a id="weNeedMoreFirepower"></a>4.3.3. We need more firepower!

The vanilla version of _Fallout 3_ is somewhat limited regarding weapons. We'll have plenty of firepower, but the weapon effects are dull, and the customization options are basically zero. Moreover, if you are used to traditional FPSs, you will sure find the aiming system a fucking crap.

We are getting serious here, because, at the end of the chapter, we will have a completely revamped weapon system in the game. As usual, Gopher has a fantastic video [covering weapon mods](https://www.youtube.com/watch?v=Vli2y7ZDUbo) (15:02), although not all of them.

We are going to install [_Weapon Mod Kits_](http://www.nexusmods.com/fallout3/mods/3388/?) (WMK), [_Energy Visuals Enhanced_](http://www.nexusmods.com/fallout3/mods/8340/?) (EVE) and [_Rogue Hallow's Ironsights_](http://www.nexusmods.com/fallout3/mods/6938/?) (RH_ironsights), along with the corresponding Paradox Ignition merged patches. This is going to throw a lot of files in our data folder, so, let's get started.

1. Download the following WMK files with NMM:
	* _Weapon Mod Kits_
	* _WMK Broken Steel Compatibility Patch_
	* _WMK Mothership Zeta Compatibility Patch_
	* _WMK Operation Anchorage Compatibility Patch_
	* _WMK Point Lookout Compatibility Patch_
	* _WMK The Pitt Compatibility Patch_
2. Download _EVE 099_ file for EVE with NMM. Ignore the optional files.
3. Download the following RH_IronSights files with NMM:
	* _RH\_IronSights BETA_
	* _RH\_IronSights BETA Update 1_
	* _New Weapons for BETA_
	* _RH\_IronSights - Better Uniques_
4. We have a good bunch of mods ready to be installed.
![!NMM weapon mods ready](Images/NMM%20weapon%20mods%20ready.png)
5. Install WMK and all its compatibility patches (the main file first and then the patches, in any order you like). Answer _Yes to all_ when asked for overwriting files (all from the previous FWE installation).
6. Install EVE. Again, it's going to overwrite several FWE files.
7. Install RH_IronSights (main file, update and optionals, in this order). Answer _Yes to all_ when asked to overwrite files, as usual.
8. Download the merged path for RH_IronSights (_RH\_Ironsights Merged_) from [Paradox Ignition page](http://www.nexusmods.com/fallout3/mods/16787/?) with NMM.
9. Close NMM and navigate to the data folder (`[%STEAM_HOME%\steamapps\common\Fallout 3 goty\Data]`) to move the following files to a folder of your choice (say, `[RH_IronSights Backup]`):
	* `RH_IronSights_Basic_VanillaPlugin.esp`
	* `RH_IronSights_Basic_AnchoragePlugin.esp`
	* `RH_IronSights_Basic_PittPlugin.esp`
	* `RH_IronSights_Basic_BrokenSteelPlugin.esp`
	* `RH_IronSights_Basic_PointLookoutPlugin.esp`
	* `RH_IronSights_Basic_ZetaPlugin.esp`
	* `RH_IronSights_Pitt_NewRifleSights.esp`
	* `RH_IronSights_RemoveReticule.esp`
	* `RH_IronSights_PL_NewItems.esp`
	* `RH_IronSights_Vanilla_BetterUniques.esp`
	* `RH_IronSights_Vanilla_NewWeapons.esp`
10. Run NMM again and install _Paradox Ignition presents The Mergers - RH\_Ironsights Merged_. The merged patch overwrites some files from the original installation to correct/update them, so let it be.
11. Run LOOT to rearrange your load order. This should be your setup by now.
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
	* `EVE.esm`
	* `RH_IRONSIGHTS.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `CASM.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `DarNifiedUIF3.esp`
	* `WeaponModKits.esp`
	* `WeaponModKits - BrokenSteel.esp`
	* `WeaponModKits - OperationAnchorage.esp`
	* `WeaponModKits - Zeta.esp`
	* `WeaponModKits - ThePitt.esp`
	* `WeaponModKits - PointLookout.esp`
12. According to LOOT, the file `RH_IRONSIGHTS.esm` is dirty, so proceed to clean it up with FO3Edit. Remember: select just that file and the files it depends on will be automatically loaded.

We have just installed a lot of overlapping mods, so we will need a compatibility patch to have them all working together. Nevertheless we have two alternatives here, both from [Blackened compatibility patches page](http://www.nexusmods.com/fallout3/mods/18173/?):

1. We can install _Blackened FWE - MMM - EVE_ and _Blackened RH\_Ironsights - FWE - EVE_ and stop installing mods right here.
2. We can install _Blackened FWE - MMM - EVE - Project Beauty_ and _Blackened RH\_Ironsights - FWE - EVE_, keepeng on installing mods from this guide, as we are going to get to Project Beauty, eventually.

This is important... If you don't want to go further, install the FWE/MMM/EVE patch, but if you want to get to the section about face-washing the game, **DON'T** install any patch yet. Take into account that you won't be able to play until a proper compatibility patch is installed, one way or another, so curb your enthusiasm.

Since I am going to deep-follow this guide (of course), I will give instructions about the RH_IronSights/FWE/EVE patch only.

1. Download and install _Blackened RH\_Ironsights - FWE - EVE_ with NMM, from [Blackened](http://www.nexusmods.com/fallout3/mods/18173/?).
2. Rearrange your load order with LOOT. Interesting changes arise:
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
	* `EVE.esm`
	* `RH_IRONSIGHTS.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `CASM.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `HZSmoothLight - FO3.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `DarNifiedUIF3.esp`
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

If you run the game, you will notice the dramatic change when aiming your weapon. **NOW**, this is serious shit.

![Fallout 3 new sights](Images/Fallout%203%20new%20sights.png)

#### <a id="expandingYourWorld"></a>4.3.4. Expanding your world

It's not that _Fallout 3 Game of the Year Edition_ lacks places to visit. On the contrary, you will be ruining your life trying to unfold the secrets of the Capital Wasteland, but, still, why not add some spice to the mix?

We are going to add three mods that add new content to the game: [_Alton, IL_](http://www.nexusmods.com/fallout3/mods/16949/?), [_Arefu Expanded_](http://www.nexusmods.com/fallout3/mods/8976/?) and [_Mothership Zeta Crew_](http://www.nexusmods.com/fallout3/mods/8747/?). Let's start.

1. Download _Alton IL Version 2-0-1_ and _Alton IL Hotfix 2-0-3_ with NMM.
2. Download _Arefu Expanded v1_7a - Data Files_ and _Arefu Expanded v1\_7d - ESP and ESM files_ with NMM.
3. Download _Mothership Zeta Crew V 166 ZIP_ with NMM.
4. Check they are all downloaded and ready in NMM. Take into account that _Mothership Zeta Crew_ is **HUGE** (over 1 GB), so be patient and make the most of your time reading online documentation about creating a book using LaTeX, for example.
![NMM new content mods](Images/NMM%20new%20content%20mods.png)
5. Activate the files in the following order, overwriting all files when necessary (the mods shouldn't overlap, except patches over original files):
	* _Alton IL - Huge World and Quest Mod - Alton IL Version 2-0-1_
	* _Alton IL Hotfix 2-0-3 RC_
	* _Arefu Expanded v1\_7d by Azar - Arefu Expanded v1\_7a - Data Files_
	* _Arefu Expanded v1\_7d by Azar - Arefu Expanded v1\_7d - ESP and ESM files_
	* _Mothership Zeta Crew - Mothership Zeta Crew V 166 ZIP_
6. When all mods are installed, fire up LOOT to rearrange your load order. This should be the load order now:
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
	* `ArefuExpandedByAzar.esm`
	* `Mothership Crew.esm`
	* `Alton, IL.esm`
	* `CRAFT.esm`
	* `FO3 Wanderers Edition - Main File.esm`
	* `FO3 Wanderers Edition - Alternate Travel.esp`
	* `CASM.esp`
	* `DarNifiedUIF3.esp`
	* `Mart's Mutant Mod - DLC Anchorage.esp`
	* `Mart's Mutant Mod - DLC Point Lookout.esp`
	* `AltonAddon.esp`
	* `FO3 Wanderers Edition - Main File.esp`
	* `FO3 Wanderers Edition - DLC Broken Steel.esp`
	* `FO3 Wanderers Edition - DLC Anchorage.esp`
	* `FO3 Wanderers Edition - DLC Mothership Zeta.esp`
	* `FO3 Wanderers Edition - DLC Point Lookout.esp`
	* `FO3 Wanderers Edition - DLC The Pitt.esp`
	* `Mart's Mutant Mod - DLC The Pitt.esp`
	* `Mart's Mutant Mod.esp`
	* `Mart's Mutant Mod - Master Menu Module.esp`
	* `Mart's Mutant Mod - DLC Broken Steel.esp`
	* `Mart's Mutant Mod - DLC Zeta.esp`
	* `Mart's Mutant Mod - FWE Master Release + DLCs.esp`
	* `Mart's Mutant Mod - FWE Master Release + Project Beauty.esp`
	* `ArefuExpandedByAzar-Radio.esp`
7. Launch the game and wait a few moments to see two reminders about _Alton, IL_ and _Arefu Expanded_ (there's no mention about _Mothership Zeta Crew_, as the mod kick-in is embedded in-game).
![Fallout 3 Arefu Expanded installed](Images/Fallout%203%20Arefu%20Expanded%20installed.png)
![Fallout 3 Alton IL installed](Images/Fallout%203%20Alton%20IL%20installed.png)




## <a id="resources"></a>5. Resources

This is a comprehensive list of the resources used throughtout this guide.



### <a id="tools"></a>5.1. Tools

* [Nexus Mod Manager](http://www.nexusmods.com/games/mods/modmanager/?). This is the tool of choice when it comes to keep all your mods organized and up-to-date.
* [LOOT](https://loot.github.io/). Installing mods on Bethesda games can be a pain in the ass, especially if you try to install a lot of possibly-colliding mods. This tool keeps the load order straight.
* [FO3Edit](http://www.nexusmods.com/fallout3/mods/637/?). _Fallout 3_ itself comes out-of-the-box with certain errors in the main and DLC files, and this tool comes in handy to correct them. Besides, this is **THE** tool to create a merged patch to run the game with an absurd amount of mods.



### <a id="guides"></a>5.2. Guides

* [Guide to fix the game in order to run under modern versions of Windows](http://steamcommunity.com/sharedfiles/filedetails/?id=149946772).
* [Why the game crashes if it runs in a box with multiple cores](http://www.sevenforums.com/gaming/20199-fallout-3-windows-7-w-quad-core.html).
* [TES5Edit cleaning guide](http://www.creationkit.com/index.php?title=TES5Edit_Cleaning_Guide_-_TES5Edit).
* [_Fallout 3_ Tweaking Guide](http://www.tweakguides.com/Fallout3_1.html).



### <a id="mods"></a>5.3. Mods

This is the list of mods used throughout this guide, in ascending alphabetical order.

* [_Adjustable HUD_](http://fallout3.nexusmods.com/mods/15886) or aHUD.
* [_Alton IL_](http://www.nexusmods.com/fallout3/mods/16949/?).
* [_Arefu Expanded_](http://www.nexusmods.com/fallout3/mods/8976/?).
* [_Better High Detail Map and Icons_](http://www.nexusmods.com/fallout3/mods/16898/?).
* [_Community Ammunition Library_](http://www.nexusmods.com/fallout3/mods/3447/?) or CALIBR.
* [_Darnified UI_](http://forums.bethsoft.com/topic/1085562-wipzbeta-darnified-ui-f3/) or DarnUI.
* [_DarnUI compatibility patch for FWE_](http://fallout3.nexusmods.com/mods/2761).
* [_Dynavision_](http://fallout3.nexusmods.com/mods/17876/).
* [_Energy Visuals Enhanced_](http://fallout3.nexusmods.com/mods/8340) or EVE.
* [_Enhanced Night Sky_](http://www.nexusmods.com/fallout3/mods/442/?).
* [_EVE compatibility patch for FOIP_](http://fallout3.nexusmods.com/mods/15961).
* [_Fake Fullscreen Mode Windowed - Alt Tab Fix_](http://www.nexusmods.com/fallout3/mods/16001/?)
* [_Fallout 3 - HD Audio Overhaul - v1.21_](http://www.nexusmods.com/fallout3/mods/13055/?)
* [_Fallout 3 re-animated_](http://fallout3.nexusmods.com/mods/7670).
* [_Fallout 3 redesigned_](http://fallout3.nexusmods.com/mods/6341).
* [_Fallout 3 Wanderers Edition_](http://www.nexusmods.com/fallout3/mods/2761/?) or FWE.
* [_Fallout Interoperability Program_](http://fallout3.nexusmods.com/mods/4968) or FOIP.
* [_Fallout Street Lights_](http://www.nexusmods.com/fallout3/mods/8069/?).
* [_Fallout Stutter Remover_](http://www.nexusmods.com/fallout3/mods/8886/?)
* [_Flora overhaul_](http://www.nexusmods.com/fallout3/mods/19864/?).
* [_Immersive HUD_](http://fallout3.nexusmods.com/mods/15790) or iHUD.
* [_krzymar HI-RES Moon_](http://www.nexusmods.com/fallout3/mods/538/?).
* [_Large Address Aware Enabler for Fallout 3_](http://www.nexusmods.com/fallout3/mods/6510/?)
* [_Lost in Light_](http://www.nexusmods.com/fallout3/mods/19163/?) or LiL.
* [_Marts Mutant Mod_](http://fallout3.nexusmods.com/mods/3211) or MMM.
* [_Mothership Zeta Crew_](http://www.nexusmods.com/fallout3/mods/8747/?)
* [_NMCS Texture Pack_](http://www.nexusmods.com/fallout3/mods/12056/?).
* [_PipBoy 3000 HD Retexture_](http://www.nexusmods.com/fallout3/mods/20373/?)
* [_Project Reality_](http://www.nexusmods.com/fallout3/mods/17418/?).
* [_Pure Water_](http://www.nexusmods.com/fallout3/mods/2599/?).
* [_RH Ironsights_](http://fallout3.nexusmods.com/mods/6938).
* [_SmoothLight - Pip-Boy Light Enhancer_](http://www.nexusmods.com/fallout3/mods/18389/?)
* [_Unofficial Fallout 3 Patch_](http://www.nexusmods.com/fallout3/mods/19122/?)
* [_User Interface Organizer_](http://www.nexusmods.com/fallout3/mods/20867) or UIO.
* [_Weapon Mod Kits_](http://fallout3.nexusmods.com/mods/3388) or WMK.



### <a id="videos"></a>5.4. Videos

These are the videos which served as spiritual inspiration author of this guide. That's me.

* [Fallout 3 : To ENB or not to ENB](https://www.youtube.com/watch?v=BP3timf65O4) (21:36).
* [Fallout 3 Mod Clinic part 1 : Remastered, Blackened and Merged](https://www.youtube.com/watch?v=TeWV1wvg7cU) (24:12).
* [Fallout 3 Mod Clinic part 2 : RH Ironsights](https://www.youtube.com/watch?v=fHbJjkBSD4g) (16:33).
* [FALLOUT 3 Mod Clinic#3: UIO - User Interface Organizer](https://www.youtube.com/watch?v=bTlXOqV6pBA) (4:42).
* [Fallout 3 Multicore Crash Fix](https://www.youtube.com/watch?v=gIY2J6W8FBU) (03:17).
* [Fallout 3 Script Extender : FOSE (Installing and using)](https://www.youtube.com/watch?v=QK_f4vHiutA) (10:07).
* [Fallout New Vegas Mod Clinic #24 : UIO - User Interface Organizer](https://www.youtube.com/watch?v=qSA2BFQ2zc4).
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