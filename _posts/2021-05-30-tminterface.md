---
layout: post
title:  TMInterface Beta
date:   2021-05-30 23:00:13 +0200
permalink: tminterface
---

### What is TMInterface?
TMInterface is a state-of-the-art TAS tool for Trackmania Nations and United Forever. It allows you to replay, analyze and modify runs to achieve faster runs and push the game to its limits.  It was never meant to be a tool for cheating or unfair play and this is why it comes with security features that doesn't allow for this. **Do not** ever attempt to drive legitimate runs and compete on public leaderboards while running the game with the tool injected. Any run done with the tool  is as a tool assisted run, regardless if the tool injected inputs or not.

<div style="display: flex;">
    <form action="https://github.com/donadigo/donadigo.github.io/raw/master/data/TMInterfaceBeta_Setup_1.0.0.exe" style="margin-right: 20px;">
        <input type="submit" class="download-button button-cyan" value="Download the newest version"/>
    </form>

    <form action="https://discord.gg/tD4rarRYpj">
        <input type="submit" class="discord-button" value="Discord"/>
    </form>
</div>

### How do I use it?
TMInterface bases off everything on console commands, much like Source games such as CS:GO. From setting the speed of the game, to setting up a bruteforce script. You can toggle the console by pressing the tilde `~` key. Script files are stored in `C:\Users\username\Documents\TMInterface\Scripts`. **Launch the tool for it to create this folder, if it does not exist.** There you can create new script files that contain your inputs/other commands that are available with TMInterface. You can open this directory by typing `open_scripts_folder` and hitting enter. Type `help` to get list of all the commands available and their short description. Type `vars` to see all variables you can set. You can check out all available commands & variables [here](https://github.com/donadigo/TMInterfacePublic/blob/master/docs.md).

The `config.txt` in `C:\Users\username\Documents\TMInterface` file enables you to run a set of commands at the beginning of TMInterface startup. In there, you can put commands like `bind r replay` to bind the R key to the command `replay` permanently.

### Downloads
Head to the top of the page to download the installer for the newest version. If you cannot use the installer for some reason (strongly recommended!), [download the raw .zip installation files](https://github.com/donadigo/donadigo.github.io/raw/master/data/TMInterfaceBeta_1.0.0.zip).

### Useful commands
* `set speed 5` - Sets the global game speed to 5x the normal speed.
* `replay` - Choose a replay in the Edit Replays menu -> Launch -> Validate and type `replay` in the console to load all the inputs of the replay you just validated. Now, load the map the replay was driven on and see all the inputs being replicated.
* `dump_inputs` - Choose a replay in the Edit Replays menu -> Launch -> Validate and type `dump_inputs` in the console to print all the inputs of the replay you just validated. The text is automatically copied into the clipboard for easy access.
* `toggle_inputs` - Toggle a live input widget display, visualizing currently loaded inputs.
* `map` - Load a map immediately from maps available in the `TrackMania` documents folder.
* `bind` - Bind a key to a command e.g: `bind f2 set speed 2`
* `load_infinity` - Loads TMInfinity into the game instance. Only available in the choose profile menu at game startup.

### Common questions
* **Q:** Is TMInterface compatible with Competition Patch?<br>
**A:** Yes, TMInterface can be installed alongside the Comeptition Patch.

* **Q:** The analog steering/acceleration does not work.<br>
**A:** All actions need to be bound in the inputs menu ingame. While running TMInterface, you need to connect a controller device to replicate analog input. If you don't own a controller, you can use software like [VJoy](https://sourceforge.net/projects/vjoystick/) to emulate it.<br>

* **Q:** The input is not injected at all.<br>
**A:** In the game launcher, Configure -> Advanced -> Inputs -> make sure that "*Alternate method*" is **unchecked**. If it still does not work, make sure that the `execute_commands` variable is `true`. You can do that by executing `set execute_commands true`.

* **Q:** "Game is not compatible with TMInterface" error<br>
**A:** It is recommended to use a standalone version of the game available [here](https://nadeo-download.cdn.ubi.com/trackmaniaforever/tmnationsforever_setup.exe).

### Tutorials
*Soon!*

### Planned features
* A save state system which allows players to share state files and load them into the game
* An interactive inputs editor allowing for rapid experimentation
* Additional programs to extract input from existing game instance, running without TMInterface
* Input display customization

### Known issues
* Crashes
* Performance issues
* Cumbersome management of input displays / custom triggers
* Sticky keys in camera 7
* Incomplete server API
* Many more
