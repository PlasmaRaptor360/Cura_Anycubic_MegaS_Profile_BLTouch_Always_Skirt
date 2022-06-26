# Cura Anycubic Mega S Profile with BLTouch
Printer Profile for **only** Mega S Printers with BLTouch [knutwurst's firmware](https://github.com/knutwurst/Marlin-2-0-x-Anycubic-i3-MEGA-S/releases)
 
## Installation
Download the bltouch definition and add it to `C:\Users\<Username>\AppData\Roaming\cura\5.0\definitions`. You might need to add other files to their proper places as well if you have not already added the normal Cura Anycubic Mega S Profile.

## What this printer profile does?
To enable every setting in the materials you can install this plugin: https://marketplace.ultimaker.com/app/cura/plugins/fieldofview/MaterialSettingsPlugin

## Notes
 * Enhanced Top/Bottom Layer calculation based on the thickness of the "Layer height" and "Initial Layer Height"
 * Set Tree support as standard
 * If tree support is enabled it has to touch build plate automatically
 * "Printing Temperature Initial Layer" is set 10 C° higher that "Printing Temperature" if not set from materials
 * "Speed" settings are derived from "Print Speed"
 * If "Travel Speed" is higher than 150mm/s a warning occurs
 * Combining is initially off
 * **Skirt is always enabled**
 * Set retraction speed to **60** and distance to **5**, as recommended in the [manual (digital page 30, physical page 26)](https://drive.google.com/file/d/13hGH6_5x4iELyqkURTVaChUewx2xc3V2/view)
 * Support for additional metadata for OctoPrint-Slicer Print Time Estimator https://github.com/NilsRo/OctoPrint-SlicerEstimator
 * Dynamic wall thickness dependent by nozzle diameter
 * BLTouch Bilinear before each print
 * Changed Cura settings according to [knutwurst's guide](https://github.com/knutwurst/Marlin-2-0-x-Anycubic-i3-MEGA-S/wiki/Beginner's-Guide-(English)#7-setup-slicer-cura)