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
* [4. Enhancing the game](#enhancingGame)
	- [4.1. Improving the user interface](#improvingUserInterface)
		+ [4.1.1. Building the basement](#buildingBasement)
		+ [4.1.2. Face-washing the user interface](#faceWashingUI)
* [5. Resources](#resources)
	- [5.1. Tools](#tools)
	- [5.2. Guides](#guides)
	- [5.3. Mods](#mods)
	- [5.4. Videos](#videos)

## <a id="introduction"></a>1. Introduction

We, human beings, have a strange knack for imagining Doomsday. We like to depict our planet devastated by plagues, war (either biological or nuclear), alien attacks or all together at the same time.

One of the videogames that best shows how could be our world after a nuclear holocaust is _Fallout 3_. And [I'm not the only one](https://warisboring.com/why-fallout-is-the-best-nuclear-war-story-ever-told-5910918d28e4) with that feeling.

However, if you have been around the videogame scene for a while, you will know that _Fallout_ games can be completely enhanced using _mods_... Well, that is a complete understatement, as you could play a whole different game with the appropriate mods. Or you could break the game. That's the tricky part.

Getting right to the point, vanilla _Fallout 3_ sucks in many different ways. You cannot even run the game if your box uses Windows 7 or higher. A lot of tinkering has to be done for the game to run flawlessly.

There is an awesome [guide to fix the game in order to run under modern versions of Windows](http://steamcommunity.com/sharedfiles/filedetails/?id=149946772), written by [BenWah](http://steamcommunity.com/id/benwaa), which I intend to follow. And there are [a hell of a lot of videos by Gopher](https://www.youtube.com/channel/UC1CSCMwaDubQ4rcYCpX40Eg) with the best _Fallout 3_ mods your money can buy (well, sort of). Give credit when credit is due, you know.

So, there is no original work here, just an extended guide to put things into perspective. And this perspective is divided into two parts:

1. The firs part is about _fixing_ the game. At the end of this chapter, you will have a flawless _Fallout 3_ game, running smoothly, with no CTD's (_Crash to Desktop_ in jargon), but it will be a vanilla game, at least content, graphics and audio-wise. No changes will be made to the story or the way you perceive the Wasteland.
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

* Is flawless (well, almost).
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

_Fallout 3_ suffers from stuttering, this is, there are certain points in the game where the visuals are lacking in fluidity. Although this can be reduced by optimizing your system (updating your graphics driver to the top, unfragmenting the hard drive, and son on), there is still a micro-stuttering that can be perceived in lower-spec machines when framerate suddenly changes.

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
7. CASM is configurable through an in-game option in your Pip-Boy 3000 (you will get your own Pip-Boy at the age of 10). Fire up your Pip-Buy by pressing <kbd>TAB</kbd> and navigate to the _Aid_ section. You will see an "item" called _CASM Options Menu_.
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

#### <a id="faceWashingUI"></a>4.1.2. Face-washing the user interface

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
13. Remember when we said "no" to use the fonts provided by DUIF3? There is an error in NMM, possibly related to modifying files in certain protected Windows folders, which crashes the program. So, go back to the [DUIF3 page](http://forums.bethsoft.com/topic/1121454-wipzbeta-darnified-ui-f3/) and copy the text block starting with `[Fonts]`. I have made half the job for you, even.
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

* [Adjustable HUD](http://fallout3.nexusmods.com/mods/15886) or aHUD.
* [Alton IL](http://www.nexusmods.com/fallout3/mods/16949/?).
* [Arefu Expanded](http://www.nexusmods.com/fallout3/mods/8976/?).
* [Better High Detail Map and Icons](http://www.nexusmods.com/fallout3/mods/16898/?).
* [Blackened](http://www.nexusmods.com/fallout3/mods/18173/?).
* [Community Ammunition Library](http://www.nexusmods.com/fallout3/mods/3447/?) or CALIBR.
* [Darnified UI](http://forums.bethsoft.com/topic/1085562-wipzbeta-darnified-ui-f3/) or DarnUI.
* [DarnUI compatibility patch for FWE](http://fallout3.nexusmods.com/mods/2761).
* [Dynavision](http://fallout3.nexusmods.com/mods/17876/).
* [Energy Visuals Enhanced](http://fallout3.nexusmods.com/mods/8340) or EVE.
* [Enhanced Night Sky](http://www.nexusmods.com/fallout3/mods/442/?).
* [EVE compatibility patch for FOIP](http://fallout3.nexusmods.com/mods/15961).
* [Fake Fullscreen Mode Windowed - Alt Tab Fix](http://www.nexusmods.com/fallout3/mods/16001/?)
* [Fallout 3 re-animated](http://fallout3.nexusmods.com/mods/7670).
* [Fallout 3 redesigned](http://fallout3.nexusmods.com/mods/6341).
* [Fallout 3 Wanderers Edition](http://www.nexusmods.com/fallout3/mods/2761/?) or FWE.
* [Fallout Interoperability Program](http://fallout3.nexusmods.com/mods/4968) or FOIP.
* [Fallout Street Lights](http://www.nexusmods.com/fallout3/mods/8069/?).
* [Fallout Stutter Remover](http://www.nexusmods.com/fallout3/mods/8886/?)
* [Flora overhaul](http://www.nexusmods.com/fallout3/mods/19864/?).
* [Immersive HUD](http://fallout3.nexusmods.com/mods/15790) or iHUD.
* [krzymar HI-RES Moon](http://www.nexusmods.com/fallout3/mods/538/?).
* [Large Address Aware Enabler for Fallout 3](http://www.nexusmods.com/fallout3/mods/6510/?)
* [Lost in Light](http://www.nexusmods.com/fallout3/mods/19163/?) or LiL.
* [Marts Mutant Mod](http://fallout3.nexusmods.com/mods/3211) or MMM (through [The Mergers](http://www.nexusmods.com/fallout3/mods/16787/?)).
* [Mothership Zeta Crew](http://www.nexusmods.com/fallout3/mods/8747/?).
* [NMCS Texture Pack](http://www.nexusmods.com/fallout3/mods/12056/?).
* [Project Reality](http://www.nexusmods.com/fallout3/mods/17418/?).
* [Pure Water](http://www.nexusmods.com/fallout3/mods/2599/?).
* [RH Ironsights](http://fallout3.nexusmods.com/mods/6938) (through [The Mergers](http://www.nexusmods.com/fallout3/mods/16787/?)).
* [Sydney Follower](http://www.nexusmods.com/fallout3/mods/9320/?).
* [Unofficial Fallout 3 Patch](http://www.nexusmods.com/fallout3/mods/19122/?)
* [User Interface Organizer](http://www.nexusmods.com/fallout3/mods/20867) or UIO.
* [Weapon Mod Kits](http://fallout3.nexusmods.com/mods/3388) or WMK.


### <a id="videos"></a>5.4. Videos

These are the videos which served as spiritual inspiration for the humble author of this awesome guide.

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