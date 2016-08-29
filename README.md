# 3D Printing at TheLab.ms

 * [3D Printing Cheat Sheet](https://github.com/TheLab-ms/3d-printing/wiki/TheLab.ms's-3D-Printing-Cheat-Sheet)
 * [Slic3r Config Bundle](https://github.com/TheLab-ms/3d-printing/blob/master/Slic3r_config_bundle.ini)
 
 
  ## **In General, pre-steps**: 
  
  > Acquire a 3D model (a STL file) of what you want to print
  > Take STL file, feed to Slic3r, export g-code with correct settings
  > Feed g-code to printer
 
 
  *A note on directions* - left/right extruders are the same left/right when physically FACING the front of the printer, looking into it
 
 ## **STEP ONE**: Acquire or create and STL file

You can acquire an STL file created by someone else on websites like [Thingiverse](http://thingiverse.com).

Some simple models to try for your first 3D print:

 * [TheLab.ms Keystand](http://www.thingiverse.com/thing:1199757)
 * [Marvin Keychain](http://www.thingiverse.com/thing:215703)
 * [5mm Calibration Cube Steps](http://www.thingiverse.com/thing:24238)
 * [SHARKZ](http://www.thingiverse.com/thing:910216)

## **STEP TWO**: Slice your STL file

We have a [configuration bundle for Slic3r](https://github.com/TheLab-ms/3d-printing/blob/master/Slic3r_config_bundle.ini) that is all set up for use with our FlashForge Creator Pro printers.  

**Don't go through Slic3r's configuration wizard.**  Just cancel it.  

You'll want to hit **"File->Load Config Bundle"** to import our config bundle.  You'll only need to do this part once.

From this point, all you need to do is "add" your STL file to Slic3r's build plate, and hit the "export gcode" button.

 * [Slic3r Download](http://slic3r.org/download) for Linux, Mac, and Windows
      * [Getting Slic3r](http://manual.slic3r.org/getting-slic3r/getting-slic3r) from the Slic3r manual
 * [Our Slic3r configuration bundle](https://raw.githubusercontent.com/TheLab-ms/3d-printing/master/Slic3r_config_bundle.ini)

If you're using Windows, you can follow our [Install Slic3r and Import TheLab’s Slic3r Configuration File Bundle for Windows](https://github.com/TheLab-ms/3d-printing/blob/master/Install%20Slic3r%20and%20Import%20TheLab%E2%80%99s%20Slic3r%20Configuration%20File%20Bundle%20for%20Windows.pdf) document.

Slic3r is in the package repositories of many Linux distributions.  The latest version is currently in the Ubuntu 15.10 "Universe" repository.  If you are going to install through your package manager, make sure you are actually getting the latest version.  A lot of important bugs have been fixed in the last few releases.

## **STEP THREE**: Print your gcode using Octoprint

We currently have two FlashForge Creator Pro 3D Printers.  

The one on the left is [badger1](https://badger1.thelab.lan/), and the one on the right is [badger2](https://badger2.thelab.lan/). They also have namebadges physically on the front of them so you can tell them apart!

 * badger1 [10.220.4.30:5000](http://10.220.4.30:5000)
 * badger2 [10.220.4.30:5001](http://10.220.4.30:5001)
 
 
 ## **Advanced Techniques**: Print your gcode using Octoprint
 
 

