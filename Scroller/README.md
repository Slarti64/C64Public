Welcome to the generic scrolling game engine source code.

Download source from the github link. 
https://github.com/martinpiper/C64Public 
(Download zip) 

Unzip it somewhere.

Change to the Scroller directory. 
Run buildIt.bat 

It creates a compressed Scroller.prg that can be run on a C64 or pretty much any C64 emulator.


ScrollEntry.a contains lots of documented tweak options to enable or disable (or define or undefine).
For example an enabled or defined option for Scroller_LinkedEnemyTest will look like: "Scroller_LinkedEnemyTest = 1"
A disabled or undefined option for Scroller_LinkedEnemyTest will look like: ";Scroller_LinkedEnemyTest = 1"
The ';' character is a comment character and causes that line to be ignored.
Thus to disable it or undefine it use a ';' character at the start of the line for that option.


ScrollerData.a contains lots of !bin commands near the top of the file.
Enable one of the !bin to include one of the game data files from the SEUCK directory. 


To create your own p00 game data file use the Vice C64 emulator, detach all d64 files, in SEUCK choose storage and save all data.
Then reference the saved p00 data file on your PC by putting the path to the file in one of the !bin commands in the ScrollerData.a file.
