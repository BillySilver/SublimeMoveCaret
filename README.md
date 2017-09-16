SublimeMoveCaret
================
A simple plugin for Sublime Text 2 / 3.

You can move the caret to the top / middle / bottom of the current view or just *x* lines from the current position.


Installation
------------
1. Use git:

        git clone https://github.com/BillySilver/SublimeMoveCaret.git "SUBLIMETEXT_DIRECTORY/Packages/SublimeMoveCaret"

2. Download this repository as ZIP, unzip it to "SUBLIMETEXT_DIRECTORY/Packages", and rename the directory to "SublimeMoveCaret".

##### Where is my SUBLIMETEXT_DIRECTORY?

For Sublime Text 3:

* Windows: %AppData%/Sublime Text 3/
* Linux: ~/.config/sublime-text-3/
* OS X: ~/Library/Application Support/Sublime Text 3/

For Sublime Text 2:
* Just replace "3" above with "2".

How to use
----------
Here are the default key bindings:

    { "keys": ["alt+up"], "command": "move_caret_top" },
    { "keys": ["alt+left"], "command": "move_caret_back", "args": { "nlines": 5}  },
    { "keys": ["alt+right"], "command": "move_caret_forward", "args": { "nlines": 5} },
    { "keys": ["alt+down"], "command": "move_caret_bottom"},

You can change the argument **nlines** in the commands `move_caret_back` or `move_caret_forward` to any integer you prefer.

Command `move_caret_middle` is optional. You can also add it to your key bindings. It takes no arguments.


Acknowledgments
---------------
Source: [Move cursor to top/middle/bottom of visible lines - Plugin Announcements - Sublime Forum](https://forum.sublimetext.com/t/move-cursor-to-top-middle-bottom-of-visible-lines/4586)

Arthor: [planet](https://forum.sublimetext.com/u/planet)

Date: Feb 24, 2012

> Hi,  
> I made a simple Plugin that moves the cursor to the top, middle or bottom of the screen (like VI H / M / L):
>
> **Update: ** Added two Functions for moving the cursor up/down by x lines (see key bindings).
>
> Note: The code is just a stripped down version of the commands found in the Vintage package (vintage_motions.py). To install, just save the code as a new Plugin (Tools->New Plugin...).
>
> Regards, Thorsten.
