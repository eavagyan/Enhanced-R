Enhanced-R: R Plugin for Sublime Text 2/3
=======================================

Introduction
------------
This plugin contains some simple features that helps in writing R languages:

* More comprehensive Indentation and Syntax
* Send commands to different applications such as R GUI, Terminal and [SublimeREPL](https://github.com/wuub/SublimeREPL).
* Show function hints in status bar
 
<p align="center">
<img width=300 src="https://github.com/randy3k/Enhanced-R/raw/master/status.png">
</p>



Supported Applications
---------------
* R GUI i386 and x64 for Windows and Mac
* Terminal and iTerm 2 for Mac
* Tmux and screen for Linux
* [SublimeREPL](https://github.com/wuub/SublimeREPL)

Note: For Windows, [AutoHotkey](http://www.autohotkey.com) which is an automation script is used
as a bridge between R and ST.

Key bindings
---------------
#### Sending Code (default: R)
**Keybinding:** `C-Enter`

* Send the selection to R (See settings for choosing default application)
* If no syntax is selected, it sends the whole line where the cursor stays at.
* Or if the current line ends with `{`, it finds the matching `}` and sends the whole block.

#### Changing Working Directory
**Keybinding:** `C-\`

* Change working directory to where the current working script is located

####  Sourcing file
**Keybinding:** `C-b`

* Tell R to source the working script


Settings
---------

Preferences -> Package Settings -> Enhanced R -> Settings

#### Application

* ``R: Choose Application`` in Command Palette to switch between applications.

#### Application paths

* In default, Enahnced R will search application's location automatically. You may manaully edit application's path.

#### Packages for function hints.

```
{
    // a list of packages which functions will show in the status bar
    // "default_pkgs": ["base", "graphics", "grDevices", "methods", "stats", "utils"],
}
```
