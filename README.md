# 3D Printing at TheLab.ms

* [3D Printing Cheat Sheet](https://github.com/TheLab-ms/3d-printing/wiki/TheLab.ms's-3D-Printing-Cheat-Sheet)
* [Slic3r Config Bundle](https://github.com/TheLab-ms/3d-printing/blob/master/Slic3r_config_bundle.ini)

## Where can I get help with my first prints?!

There lots of friendly people at TheLab.ms that know how to use the printers, and they'd also be happy to help you get started.  If you sign into [Slack][httpL//thelab.slack.com] and join the `3d_printing` channel.  You can make arrangements with someone there to meet you at TheLab.ms and show you the ropes.

## **In General, pre-steps**:   
- Acquire a 3D model (a STL file) of what you want to print
- Take STL file, feed to Slic3r, export g-code with correct settings
- Feed g-code to printer

 
*A note on directions* - left/right extruders are the same left/right when physically FACING the front of the printer, looking into it
 
## **STEP ONE**: Acquire or create an STL file

You can acquire an STL file created by someone else on websites like [Thingiverse](http://thingiverse.com).

Some simple models to try for your first 3D print:

 * [TheLab.ms Keystand](http://www.thingiverse.com/thing:1199757)
 * [Marvin Keychain](http://www.thingiverse.com/thing:215703)
 * [5mm Calibration Cube Steps](http://www.thingiverse.com/thing:24238)
 * [SHARKZ](http://www.thingiverse.com/thing:910216)

## **STEP TWO**: Slice your STL file

If you're using Windows -> [Install Slic3r and Import TheLab’s Slic3r Configuration File Bundle for Windows](https://github.com/TheLab-ms/3d-printing/blob/master/Install%20Slic3r%20and%20Import%20TheLab%E2%80%99s%20Slic3r%20Configuration%20File%20Bundle%20for%20Windows.pdf) 

Slic3r is in the package repositories of many Linux distributions.  The latest version is currently in the Ubuntu 15.10 "Universe" repository.  If you are going to install through your package manager, make sure you are actually getting the latest version.  A lot of important bugs have been fixed in the last few releases.

We have a [configuration bundle for Slic3r](https://github.com/TheLab-ms/3d-printing/blob/master/Slic3r_config_bundle.ini) that is all set up for use with our FlashForge Creator Pro printers.  

**Don't go through Slic3r's configuration wizard.**  Just cancel it.  

You'll want to hit **"File->Load Config Bundle"** to import our config bundle.  You'll only need to do this part once.

From this point, all you need to do is "add" your STL file to Slic3r's build plate.

Select a nozzle to extrude from (right click and hit 'settings' while highlighting the model) -

- Default = right nozzle
- 1 = right nozzle
- 2 = left nozzle


 and hit the "export gcode" button.

* [Slic3r Download](http://slic3r.org/download) for Linux, Mac, and Windows
* [Getting Slic3r](http://manual.slic3r.org/getting-slic3r/getting-slic3r) from the Slic3r manual


## **STEP THREE**: Print your gcode using Octoprint

We currently have two FlashForge Creator Pro 3D Printers.  

The one on the left is [badger1](https://badger1.thelab.lan/), and the one on the right is [badger2](https://badger2.thelab.lan/). They also have namebadges physically on the front of them so you can tell them apart!

 * badger1 [10.220.4.30:5000](http://10.220.4.30:5000)
 * badger2 [10.220.4.30:5001](http://10.220.4.30:5001)
 
 You'll be able to access these IP's via a web browser.
 
 *If not, try https://badger1.thelab.lan - you'll have to accept an invalid certificate*
 
 **login username** - thelab
 **login password** - password
 
 
 
 
 ### Before you hit that print button
- Level the plate (you'll need to be shown how to physically do this)
- Hair spray the glass plate (Both PLA and ABS plastics need this!)
- Verify you have enough plastic on the spool, and that it will feed cleanly with getting stuck
 
**Make sure it's a filament that prints at normal speed** - most filament is okay, but currently the white has to print at 80% speed. To set this up, start a print and physically go to the printer, arrow down, and select "Change Speed". For white, set it to 80%.
 
 
 ## **Advanced Techniques**: 
 
 **HELP**
 
 *During a print, the extruder is moving, but no plastic is coming out!* - Try re-leveling the plate. There is a difference between leveling a 'hot' printer and a 'cold' one because of thermal expanion with the metal nozzles expanding.
 
 **OR** Make sure you have a extruder set besides 'default' in Slic3r. (Currently unsure on this)
 
 **OR** Make sure that the nozzle isn't clogged - "load filament" on the printer and validate that it will print with the current nozzle
 
 *My file is only halfway printing!* - It may be because Slic3r only exported half of the file. If you print the item twice and it stops in the same spot, it's probably because the gcode didn't completely export. This is a known issue. Just re-export the item, and MAKE SURE it finishes exporting completely.
 
 
 
 

