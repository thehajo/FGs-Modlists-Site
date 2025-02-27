---
title: "Installation Instructions"
description: "The Masterstroke installation instructions."
lead: ""
date: 2020-10-13T15:21:01+02:00
lastmod: 2020-10-13T15:21:01+02:00
draft: false
images: []
menu:
  masterstroke:
    parent: "Masterstroke"
weight: 20
toc: true
---

## Pre-Installation

### Pagefile Configuration

Bigger Skyrim modlists need a lot of memory, and when there is not enough available it may fail allocating more. To fix this, you'll want to have a bigger pagefile.

A pagefile is a file on your disk Windows will use when there is not enough RAM available.

Never disable the pagefile - this may lead to various issues on your system, including Skyrim crashes.

To set the pagefile up properly for this modlist, follow these steps:

1. Press Windows + R on your keyboard and enter `sysdm.cpl ,3`
2. Under the Performance section, press 'Settings'
3. Go to the Advanced tab at the top, and at the Virtual memory section press 'Change...'
4. Disable 'Automatically manage paging file size for all drives'
5. Set a custom size for your fastest drive and increase the initial and maximum size to be at least 20GB (20000MB).
6. Restart your computer to make sure the changes have taken effect.

If you have more than one drive, try enabling it for at least one more drive as a backup (make sure it has a decent bit of free space, like 15GB). Set the size to 'System managed size'.

### Microsoft Visual C++

The Visual C++ Redistributable is a DLL (Dynamic Link Library) file required by programs or games built using Microsoft’s Visual Studio software development environment. As Skyrim Special Edition is a 64-bit program, elements of it - along with other aspects of the modlist - require the 64-bit version of Visual C++ in order to run.

Click the link to download the latest Visual C++ x64 Redistributable, then double-click the downloaded file and follow the instructions:

- [Microsoft Visual C++ x64](https://aka.ms/vs/16/release/vc_redist.x64.exe)



### Microsoft .Net Runtime

This is another runtime library required by some programs. Not having these installed can result in issues running Living Skyrim.

Click the link to open a page on the Microsoft Website to download the .NET runtime files. You may need both the Desktop and Console versions, so please install both:

- [.Net Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/5.0/runtime)


### Skyrim Special Edition Creation Kit.

You must now install Skyrim Special Edition Creation Kit through Steam *on the same drive as your Skyrim: Special Edition installation*. The install of the list will not proceed without it.

### Steam & SSE Setup
{{< alert context="danger" icon="🛑" >}}
**WARNING!**

Before installing Masterstroke, you should make sure Skyrim: Special Edition is up to date in Steam. If you have run a downgrade patcher or not updated yet, verifying the game files using Steam will fix any issues stemming from an out of date game you may encounter during installation.
{{< /alert >}}

Before proceeding with installation, it’s important that your Steam and Skyrim Special Edition install are configured correctly.

First, make sure that your Steam library, and therefore the Skyrim Special Edition install folder, is not located within your Program Files, Program Files (x86), Desktop, or Documents folders. Having the Steam library or your copy of Skyrim Special Edition in either of these folders is known to cause issues. For more information about how this can be problematic and how Windows protects folders, consult this link: [Click Me!](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/controlled-folders?view=o365-worldwide) Instructions on how to move your Steam library can be found elsewhere on the internet.

Next, you’ll need a clean copy of Skyrim Special Edition. To get your copy to this state, follow these steps:

1. In Steam, uninstall Skyrim: Special Edition (Right-click > Manage > Uninstall).
2. If there are any files leftover in the Skyrim Special Edition game folder (Right-click > Manage > Browse Local Files), delete them.
3. Install Skyrim: Special Edition.

{{< alert context="success" icon="📝" >}}
**Protip:** 

If you want to be absolutely certain you have uninstalled Skyrim completely, download and use Skyrim Shredder.
{{< /alert >}}


Afterwards, you need to disable automatic updates for Skyrim to avoid a game update breaking your copy of the game and therefore the modlist.

1. In Steam, set Skyrim: Special Edition to update only when opened. (Right-click > Properties… > Updates > Automatic updates > Only update this game when I launch it)
2. In Steam, disable the Steam Overlay. (Right-click > Properties… > General > Enable the Steam Overlay while in-game checkbox)

Once the above steps are completed, launch Skyrim SE through Steam to create any INI or registry entries the game needs. Immediately exit the launcher once it has successfully selected a graphics preset for your hardware. The INIs it just created will be overwritten by the ones included in the modlist, but this is a necessary step for Wabbajack to recognize that you have the game installed.

### Wabbajack Preparations
We’ll now setup the folders needed for the installation to proceed smoothly.

1. Create two empty folders: one named Wabbajack and the other named Masterstroke.
2. Ensure that these two folders are not within any of the following folders: your Skyrim Special Edition install folder, your Program Files folder, your Program Files (x86) folder, your Documents folder, your Downloads folder, or the Desktop.
3. Additionally, ensure that these two folders are not contained within each other.
4. Ensure that both the Wabbajack and Masterstroke folders are completely empty. If they are not empty, make them empty.
5. Download the latest version of Wabbajack from the Wabbajack website: [Wabbajack](https://www.wabbajack.org/#/).
6. Place the Wabbajack.exe file you just downloaded into the folder you created earlier called Wabbajack.

{{< alert context="danger" icon="🛑" >}}
**WARNING!**

**Failure to set up these folders properly will result in the install failing. For example, `[install drive]\Wabbajack\Masterstroke` is incorrect.**
{{< /alert >}}

## Installing the List
If you are updating your existing installation of Masterstroke, skip to the [Updating Masterstroke](#updating-masterstroke) section of this document.

It’s now time to begin the installation of the list. Follow these steps:

1. Run Wabbajack.exe.
2. At the bottom of the window, click Browse Modlists.
3. Locate the Masterstroke card and click the download button to download the installer file.
4. Once downloaded, click the play button.
5. Below the image you see of the Masterstroke logo, there are three text boxes. The second and third need to be filled out.
6. Click the three dots in the second (middle) box. Navigate to your Masterstroke folder and then select this folder in the window that appears. This middle box tells you where the list will be installed, including the copy of Mod Organizer 2 that you’ll need to use to launch the list.
7. The third (bottom) box will automatically populate using the folder you just selected. This third box tells you where all of the mods will be downloaded. If you have hard drive limitations, you may change this to another folder on another hard drive by clicking the three dots in this box and selecting a new folder.
8. Click the play/right arrow button to begin the installation.

{{< alert context="danger" icon="🛑" >}}
**WARNING!**

Wabbajack will prompt you to manually download mods from Lovers Lab, please make sure you have an account and are signed into Lovers Lab through Wabbajack's settings menu. Once you have logged in you will see a download button on each mod page Wabbajack shows you in it's browser, you will see a black banner at the top of each download page indicating which file you should download if the page shows multiple files available to download. **please make sure you read this and download the correct mod.**
{{< /alert >}}

| With Nexus Premium | Without Nexus Premium |
| :--- | :--- |
| 9. Wabbajack will ask you to login to Nexus and authorize your API key so it can download mods for you automatically. If this doesn’t happen, it isn’t a problem and means you’ve already set this up. | 9. Wabbajack will prompt you to click all the needed buttons to download the modlist. Be prepared for this to take an extraordinarily long time. Current reports indicate installing the list manually takes approximately 24 hours. Also be aware that due to the amount of time required when installing this list manually, the list may update during the time it takes to install and you may need to start over if that happens. Installing with Nexus Premium isn’t required, but is strongly recommended if you value your time. If you must install the list manually, put on an audiobook or a TV show and make a day of it. |
| 10. Wabbajack will now download and install all of the mods. This will take a while (3-4 hours at most). Take this opportunity to read the Important Mods You Need To Know About section of this document. | |

{{< alert context="warning" icon="⚠️" >}}
**Important!** 

Reading the Important Mods section of this document is not optional. You won't have any idea what's going on if you don't.
{{< /alert >}}

Once complete, Wabbajack will indicate it is done with a green box that says "Installation complete". You may exit Wabbajack after this appears.

If it does not complete successfully (a red box with "Installation failed"), consult the Masterstroke Troubleshooting page of this document, or visit the [Masterstroke Discord server](https://discord.gg/NdmGpGzqg8) for assistance. 

## Post-Wabbajack Install

### Mod Organizer 2
Among other things, Wabbajack has installed a copy of Mod Organizer 2 for you. This copy of Mod Organizer 2 is specific to Masterstroke and will not affect any other modlists you have installed.

1. Inside your Masterstroke folder, locate and launch ModOrganizer.exe. If this is not inside the folder, your installation has failed and you need to consult the Common Issues section of this document.
2. Mod Organizer 2 will have a dark theme already selected for you. If it does not, something has gone wrong and you will need to start over at the Installing the List section of this document.
3. A dialogue may appear and ask if you want to associate Mod Organizer with .nxm links. Click Yes. If this dialogue does not appear, it is not an issue and means you’ve likely already done this.
4. Another dialogue may appear asking you to update the game's registry path. Click Yes on this popup if it appears. If it does not appear, it is not an issue and likely means you've already done this.

{{< alert context="warning" icon="⚠️" >}}
**Important!** 

You'll notice that multiple mods in MO2 are deactivated, leave them as they are unless told otherwise!
For more information: [Click here](https://www.fgsmodlists.com/masterstroke/beforeyoustart/#optional-creature-profile)
{{< /alert >}}

### Configuration Specific

If you're using an ultrawide monitor, you can enable either of the Nordic UI Ultrawide options under the "Configuration Specific" section of the left pane of MO2. Just make sure you only enable the one that matches your monitor's resolution ratio.

### ENB

The default ENB included with Masterstroke is [Culminated ENB](https://www.nexusmods.com/skyrimspecialedition/mods/53167). Support is not provided for changing it. You may, however, disable ENB during play by loading into the game and pressing `Shift + F12`. Disabling ENB will drastically improve performance but will make the game look worse overall.

## Updating Masterstroke
If you are updating Masterstroke, the process is very similar to installing the list. Before you update, you should at a minimum backup your save files. Updating may delete any saves that are present. Additionally, make sure you are using the latest version of Wabbajack (it should automatically update itself when you launch the program).

{{< alert context="danger" icon="🛑" >}}
**WARNING!**

**Whilst some incremental list updates are save-safe, larger updates often require a brand new save file to avoid corruption. Check the newest update announcement found in the `#nsfw-announcements` channel on the Discord server before updating.**
{{< /alert >}}

1. Run Wabbajack.exe.
2. At the bottom of the window, click Browse Modlists.
3. Locate the Masterstroke card and click the download button to download the installer file.
4. Once downloaded, click the play button.
5. Below the image you see of the Masterstroke logo, there are three text boxes. The second and third need to be filled out.
6. Click the three dots in the second (middle) box. Navigate to your Masterstroke folder and then select this folder in the window that appears. This middle box tells you where the list will be installed, including the copy of Mod Organizer 2 that you’ll need to use to launch the list.
7. The third (bottom) box will automatically populate using the folder you just selected. This third box tells you where all of the mods will be downloaded. If you have hard drive limitations, you may change this to another folder on another hard drive by clicking the three dots in this box and selecting a new folder.
8. Click the play/right arrow button to begin the installation.
9. If you are prompted to overwrite, confirm that this is what you want to do by clicking the Confirm button.

## Launching Masterstroke
To actually launch and then play Masterstroke, follow these steps:

1. Launch the copy of Mod Organizer 2 found inside your Masterstroke folder.
2. In the top-right corner of Mod Organizer, you’ll see a large dropdown menu. Select Masterstroke [SKSE] from this dropdown menu.
3. Click the large Run button.
4. This is how Masterstroke should always be launched. You can create a shortcut to this selection on your desktop, if you wish, using the Shortcut button directly below the large Run button.
5. Once Skyrim starts, create a new game.
6. Create your character and name them whatever you’d like.
7. As soon as you gain control of your character, do nothing. The mods are initializing and this can take several minutes. You’ll see a list of mods appearing in the top left corner of your screen.
8. Once you see that no more items are appearing in the list in the top left, you can proceed to the next steps.

{{< alert context="danger" icon="🛑" >}}
**WARNING!**

**Loading a save from another modlist or from before you installed Masterstroke will corrupt that save, do not do this.**
{{< /alert >}}

## The MCM Settings
The MCMs are configured via MCM Recorder. See this document for information about how to set up the MCMs and create your character: [Click Here](/masterstroke/mcm)

## Bug Reporting

While we have tried out best to eliminate as many bugs and inconsistencies as possible, it is unfortunately a near certainty that at some point you will come across something that could be considered a bug. Whether it's duplicate objects overlapping, an imbalanced crafting recipe, or something else entirely, it's important that you report bugs you find so that it can be fixed for everyone.

To report a bug, follow these steps:

1.  Go to this Google Form: [Click Me!](/masterstroke/bugreport)
2.  Fill out the form and submit the form.
3.  That's it, you're done!

{{< alert context="warning" icon="⚠️" >}}
**Important!** 

If we need additional information about the bug, we will contact you via Discord.
Please make sure to enter your full Discord username (Username#XXXX).

{{< /alert >}}

