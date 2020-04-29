
SheepShaver February 1, 2014 ReadMe


This UB build was compiled from source as it existed in cebix/macemu github repository on February 1, 2014, using SDL 1.2.15.

Many thanks to the contributors who made this build possible, especially our forum members "Myrd" and "vasi".

This build works on PPC and Intel Macs, MacOSX 10.4 (Tiger) through OSX 10.9 (Mavericks).

A first install on Intel machines will run in 32-bit mode by default. In Snow Leopard on 64-bit capable machines and in Lion and later, it can be set to run in 64-bit mode by unchecking "Open in 32-bit mode" in Finder Get Info panel.

If you have an existing SheepShaver setup, you can simply replace the application with the new application.

If you set up SheepShaver for the first time, you will also need a compatible ROM file and a retail MacOS install CD (or a install CD disk image).

For other than US English keyboard layouts the included keycodes file is needed.

See the setup manual for more information.

Questions and comments please in Emaculation SheepShaver forum:
http://www.emaculation.com/forum/


Known issues

On all hosts:
When you switch from window to full-screen mode using Ctrl-Return (new feature) before you used the mouse cursor in the emulator at least once, you may loose the cursor. One click on the desktop or pressing the control key suffices to bring back the cursor.

On PPC machines:
Like previous builds, very CPU hungry. (On PPC hosts set refresh rate in SheepShaver not higher than 30Hz, preferably at 15Hz.)

On Intel machines:
After minimizing or hiding the SheepShaver window and again bringing it back in view, colors in the window will not be displayed correctly. It can be resolved by forcing the emulator to redraw its screen by changing (and changing back) the color depth setting in Monitors control panel or from the color depth control strip tile.

In full-screen mode in 64-bit mode in MacOSX 10.6 (Snow Leopard):
Serious cursor problems with clicking in the menu bar in full-screen mode. (Use SheepShaver in 32-bit mode if you want to use it full-screen.)

In OSX 10.8 (Mountain Lion) and 10.9 (Mavericks):
OSX 10.8 and later prevents mounting of physical CD-ROMs in SheepShaver. CD disk image still work fine, though. See setup manual for more information.


Improvements in 1 February 2014 build:
- Support for disk images in sparsebundle format.
- Cursor grabbing toggle (Ctrl-F5). Pressing Ctrl-F5 will make the emulator grab the mouse cursor and keep it inside its window. Especially useful for some games. Again pressing Ctrl-F5 will release the cursor.
- Window-Fullscreen toggle (Ctrl-Return). Pressing Ctrl-Return will toggle between window mode and full-screen mode.

Improvements in 15 July 2012 build:
- Gamma fix that allows running Ferazel's Wand and some other games.- When SheepShaver is not using CD-ROMs (CD-ROM driver disabled in preferences), SheepShaver will no longer prevent ejecting CD-ROMs in the OSX host.
- More reliable mounting and unmounting CD-ROMs while SheepShaver is running. (Not in Mountain Lion, see known issue above.)- Accidental mounting of disk images at the same time in SheepShaver and OSX is prevented.- In 64-bit mode, copy and paste formatted text both ways between guest MacOS and host OSX in 64-bit mode. (Tested with SimpleText and Tex-Edit Plus in MacOS and with TextEdit in OSX. It may work with more applications.)
- Copy and paste images now also in 64-bit mode, both ways between guest MacOS and host OSX.

Improvements in 11 February 2012 build:
- Now uses the preferred "hardware cursor" in all MacOSX versions
- Better stability in 64-bit mode
- No odd "unexpectedly quit" message at startup on PPC

Improvements in 6 November 2010 build:
- Will not try to run in 64-bit mode in Leopard.

Improvements in 24 October 2010 build:
- Will now run in 64-bit mode in Snow Leopard on 64-bit able Intel Macs
- Multiple related 'under the hood' changes.
- Partial support for bin/cue files to enable the use of (images of) mixed
digital/audio cdroms.

Improvements in 25 October 2009 build:
- Fix for freeze or crash at startup on some host machines that was introduced in the previous build.

Improvements in 18 October 2009 build:
- "Cannot map RAM" error on Leopard fixed
- The emulated machine can now use more than 512 MB of RAM
- When a rom file is not set in preferences, a rom file in the current directory with default name "Mac OS ROM" or "ROM" will now always be found (not only on first boot)
- A crash that could occur while booting a new virtual/emulated machine (creating a new nvram file) with MacOS 7.5 fixed
- Support for self-contained virtual machine bundles with extension .sheepvm
- Removed audio patch (still in cvs) that caused degradation of sound performance rather than the intended improvement
- Problems with copy and paste of styled text in some applications fixed

Improvements in 19 March 2009 (full-screen) build:
- Full-screen support
- Possible improvement of sound performance on slow host machines

Improvements in 21 July 2008 build:
- Mouse buttons correctly numbered
- If no ROM can be opened, SheepShaver will quietly quit instead of hang
- Refresh Rate "Dynamic" sets correctly frameskip to "0" and is now the preferred setting on fast host machines

Some of the earlier improvements since the latest 'official' release version (2.3-Pre, 14 May 2006):
- Greatly improved performance on Intel machines (JIT compiler)
- Correct handling of resource forks and TYPE/CREATOR codes of files transferred through the shared folder (Unix Root)
- Corrected cursor placement and display of colored cursors
- Built-in Preferences editor


Disclaimer:
I am not a software developer, I do not have programmer skills, I am just a user, a hobbyist, like you probably are. I built the application from the source code, written by others, as it is available cebix/macemu github repository. I can give no guarantee that this software will work or that this software will not damage your files or your system. If you use this software, all possible consequences are your own responsibility.


01 February 2014
Ronald P. Regensburg
Amsterdam, Netherlands
