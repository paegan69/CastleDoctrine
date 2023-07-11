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

Coming Soon.

Win32
-----
1. Download the MinGW Installer [here](https://sourceforge.net/projects/mingw/).
2. Run the installer and select mingw-developer-tool, mingw32-base, mingw32-gcc-g++, and msys-base.
3. Go to https://www.libsdl.org/release/, download SDL-devel-1.2.15-mingw32.tar.gz and extract to a temp folder.
4. From your temp(~temp) folder, copy to your MINGW installation (~wingw):
     a. ~temp\SDL-1.2.15\include\SDL\ to ~mingw\include\SDL\
     b. ~temp\SDL-1.2.15\lib\ to ~mingw\lib\
     c. ~temp\SDL-1.2.15\bin\sdl-config to ~mingw\bin\sdl-config
     d. ~temp\SDL-1.2.15\bin\SDL.dll to Windows\System32 and Windows\SysWOW64
5. Run ~mingw\msys\1.0\msys.bat



Release Notes
-------------
Make sure you have the dev package of the following library installed:
- [libsdl](http://www.libsdl.org/)

The included "runToBuild" script should build the game for you automatically.
