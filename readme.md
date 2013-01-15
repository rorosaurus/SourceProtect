#AdBlock & Protection for TF2

## Message from CasualX

*September 11th, 2012*

Hello, since recently an exploit was discovered to execute arbitrary commands on clients (fixed in yesterday's update) I decided to see what could be done about this with purely cfg scripts to protect against this.

## Features

*	Protection against an invasive server anti-cheat (taking & uploading screenshots behind your back). Now useless because of the update.
*	AdBlocks against pinion motd adverts (Stops the 'You may close the MOTD in 5 seconds'!).
*	Prevents servers from playing sounds on your client.
*	There are some commands the server is allowed to execute, I don't see why the server needs access & blocked it.

## Download

Download from the Github repository [here](https://github.com/CasualX/SourceProtect).  Click the 'ZIP' button in the description.

## Installation

Extract protect.cfg to

    C:/Program Files/Steam/Steamapps/USERNAME/Team Fortress 2/tf/cfg

or a similar folder in your configuration.

Ensure you have a file with the name autoexec.cfg in this directory.  If you have no such file, create an empty file in Notepad and ensure you save it with the .cfg extension.  Add a new line to your autoexec.cfg file with the text

    exec protect.cfg

Next, you must create an empty file in your

    C:/Program Files/Steam/Steamapps/USERNAME/Team Fortress 2/tf

or similar directory named textwindow_temp.html.  Ensure this file is read-only by right clicking, selecting Properties, ticking the "Read-Only" box, and clicking OK or Apply.

Open your hosts file in Notepad.  You can easily navigate to the directory containing the hosts file by pressing Windows+R and pasting

    %SystemRoot%/system32/drivers/etc/

Navigate to Notepad in your Start menu and run it as an Administrator by selecting that option from the right-click menu.  Drag the hosts file from the directory we just opened into Notepad.  Add the following line to the end

    127.0.0.1 motd.pinion.gg

Save the file when you are done.

## Use

This configuration cannot remove the message telling you to wait.  Instead, it blocks the MOTD from popping up - this allows you to ignore what it says and play while the timer instructs you to wait.