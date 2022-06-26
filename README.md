# Cura Anycubic MegaS Profile
Printer Profile for **only** Mega S Printers 
 
## Installation
Download the files and move the files to the Cura installation folders like C:\Program Files\Ultimaker Cura 4.8.0\resources. Under windows you can also use the AppData folder within your profile like C:\Users\<Username>\AppData\Roaming\cura\4.8

Profiles are integrated in Cura 4.10 and newer by default but it has to be integration with the standard release cycle. So here you can get the newest version.

## What this printer profile does?
I created this printer profile because the one contained in Cura 4.8 does not support central settings. The standard dependency in Cura is Printer Settings -> Material Settings -> Quality Settings. So I moved every configuration to the printer.

To enable every setting in the materials you can install this plugin: https://marketplace.ultimaker.com/app/cura/plugins/fieldofview/MaterialSettingsPlugin

## Notes
 * Enhanced Top/Bottom Layer calculation based on the thickness of the "Layer height" and "Initial Layer Height"
 * Set Tree support as standard
 * If tree support is enabled it has to touch build plate automatically
 * "Printing Temperature Initial Layer" is set 10 C° higher that "Printing Temperature" if not set from materials
 * "Speed" settings are derived from "Print Speed"
 * If "Travel Speed" is higher than 150mm/s a warning occurs
 * Combining is initially off
 * If support is enabled "Build Plate Adhesion Type" will still be set to Skirt
 * GCode Start script is changed to support initial print and bed temperatures (parallel heatup)
 * Set retraction speed to **60** as this is the max. firmware setting. Maximum value constraint to 40, but has to be enabled in firmware.
    * Change retraction distance as well to 5mm, as recommended in the [manual (digital page 30, physical page 26)](https://drive.google.com/file/d/13hGH6_5x4iELyqkURTVaChUewx2xc3V2/view)
 * Support for additional metadata for OctoPrint-Slicer Print Time Estimator https://github.com/NilsRo/OctoPrint-SlicerEstimator
 * Dynamic wall thickness dependent by nozzle diameter
 * BLTouch Bilinear before each print
 * Changed Cura settings according to [knutwurst's guide](https://github.com/knutwurst/Marlin-2-0-x-Anycubic-i3-MEGA-S/wiki/Beginner's-Guide-(English)#7-setup-slicer-cura)
    * Using knutwurst firmware as well