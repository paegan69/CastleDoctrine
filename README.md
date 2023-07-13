CastleDoctrine
==============

[Castle Doctrine](http://thecastledoctrine.net/) - [Jason Rohrer](http://hcsoftware.sourceforge.net/jason-rohrer/)'s tenth game. A massively-multiplayer game of burglary and home defense. Available now.  

- Buy direct: http://thecastledoctrine.net/
- Buy on Steam - https://store.steampowered.com/app/249570/The_Castle_Doctrine/

A fork of the original code by Rohrer, trying to apply code updates so:
1. Server php is compatible with PHP 7+
2. Win32 executables can be compiled on Linux systems.
3. Updated compilation of OSX binaries possible

Compile Instructions
--------------------
Linux
-----

1. Make a new directory (e.g. `mkdir cdoctrine`)
2. Clone the repo using gh or git (e.g `git clone https://github.com/paegan69/CastleDoctrine cdoctrine/`) or download the repo and extract to the created dir.
3. Install the g++ compiler (`sudo apt install build-essential`)
4. Install the MinGW compiler (`sudo apt-get install gcc-mingw-w64`) n.b. this may only be needed to compile Windows binaries.
5. Install the SDL libraries (`sudo apt-get install libsdl1.2-dev`)
6. Install ImageMagik (`sudo apt install imagemagick`)
7. `cd cdoctrine`
8. `sudo chmod -R 777 ./minorGems`
9. `chmod 777 runToBuild`
10. Execute runToBuild
11. $$ Profit? $$

Win32
-----
1. Download the MinGW Installer [here](https://sourceforge.net/projects/mingw/).
2. Run the installer and select mingw-developer-tool, mingw32-base, mingw32-gcc-g++, and msys-base.
3. Go to https://www.libsdl.org/release/, download SDL-devel-1.2.15-mingw32.tar.gz and extract to a temp folder.
4. From your temp(~temp) folder, copy to your MINGW installation (~mingw):
     a. ~temp\SDL-1.2.15\include\SDL\ to ~mingw\include\SDL\
     b. ~temp\SDL-1.2.15\lib\ to ~mingw\lib\
     c. ~temp\SDL-1.2.15\bin\sdl-config to ~mingw\bin\sdl-config
     d. ~temp\SDL-1.2.15\bin\SDL.dll to Windows\System32 and Windows\SysWOW64
5. Download a copy of the repo and extract it to a working folder(~cdoctrine)
6. Run ~mingw\msys\1.0\msys.bat
7. In the new console window change your working directory to the newly created working folder (cd ~cdoctrine)
8. Execute runToBuild
9. $$ Profit? $$

MacOSX
------
No freaking clue when.

Release Notes
-------------
Make sure you have the dev package of the following library installed:
- [libsdl](https://www.libsdl.org/release/SDL-devel-1.2.15-mingw32.tar.gz)

The included "runToBuild" script should build the game for you automatically.

Known Bugs
----------
Currently does not create a Windows executable in a Linux build environment. Unable to path `windows.h`.
