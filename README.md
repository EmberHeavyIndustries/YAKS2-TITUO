# YAKS2 - TITUO


**If you like this project and want to contribute to its further development, please consider donate some $ or € (paypal friends & family, please or DO NOT select "Buying something" from money transfer frontpage).** 

| [![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://paypal.me/EmberHeavyIndustries)||[![Email, Contacts & Requests](https://github.com/EmberHeavyIndustries/Depot/blob/master/Pics/EmailSticker.jpg?raw=true)](mailto:EmberHEavyIndustries@gmail.com)|
| ------------------------------ | ---------------------------------------------- | --------------------------- |


[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)


**YAKS2-TITUO** is an **"Intelligent" kickstart switcher** for the Amiga A500-A600-A2000 and A1200-A4000, with unique features:

- A500/A600/A2000 version
  - Can switch among four or eight different kickstarts
  - Kickstarts can be flashed at any time by mean of YAKS2 adapter and any common chip flasher, capable of managing 29F080 chips
  - Kickstart selection by mean of CTRL-A-A without the need of any additional wiring inside Amiga
  - Keep track of the selected kickstart upon poweroff
  - Optional audible kickstart selection confirmation 

- A1200/A4000 version
  - Can switch among two or four different kickstarts
  - Kickstarts must be flashed before board assembling (not re-flashable)
  - Kickstart selection by mean of CTRL-A-A without the need of any additional wiring inside Amiga
  - Keep track of the selected kickstart upon poweroff
  - Optional audible kickstart selection confirmation 

## YAKS2-TITUO FLAVORS

The kickswitcher comes in three differen flavors, according to intened use and user preferences:


### **YAKS2-TITUO R02.1**

- Suitable for A500, A600, A2000
- Kickstart images can be flashed at any time (by mean of YAKS2->29F080 adaptor)
- Firmware can be upgraded via ICSP
- Kickstart selection by CTRL-A-A and RST methods (can be easily modded for AUTOSENSE - 1 wire mod)
- Onboard buzzer for audible kickstart switch and named selection evidence
- "D" shaped footprint
- Can switch among 4-kickstart-images or 8-kickstart-images

![R02.1](https://github.com/EmberHeavyIndustries/YAKS2-TITUO/blob/master/Pics/YAKS2-TITUO_300.jpg)





### **YAKS2-TITUO R03.1al**

- Suitable for A500, A600, A2000
- Kickstart images can be flashed at any time (by mean of YAKS2->29F080 adaptor)
- Firmware cannot be upgraded via ICSP
- Kickstart selection by CTRL-A-A, support both AUTOSENSE (no additional wires) and RST methods
- Can connect an external buzzer for audible kickstart switch and named selection evidence
- Visible kickstart switch and named selection evidence
- Small footprint
- Can switch among 4-kickstart-images or 8-kickstart-images

![R03.1al](https://github.com/EmberHeavyIndustries/YAKS2-TITUO/blob/master/Pics/YAKS2-TITUO-AL_300.jpg)





### **YAKS2-TITUO R03.1bl**

- Suitable for A1200 and A4000
- Kickstart images cannot be re-flashed 
- Firmware cannot be upgraded via ICSP
- Kickstart selection by CTRL-A-A, support both AUTOSENSE (no additional wires) and RST methods
- Can connect an external buzzer for audible kickstart switch and named selection evidence
- Visible kickstart switch and named selection evidence
- Small footprint
- Can switch among 2-kickstart-images or 4-kickstart-images

![R03.1al](https://github.com/EmberHeavyIndustries/YAKS2-TITUO/blob/master/Pics/YAKS2-TITUO-BL_300.jpg)

/*************** EDITING IN PROGRESS *************************/



### **EAGLE SCHEMATICS, BOARD LAYOUT and GERBER FILES**

All schemtacis, layouts, gerber files and BOM are in 'Docs' subdirectory

### **FIRMWARE**

Preferred firmware can be downloaded from 'Firmware' subdirectory


## **LICENSE TERMS**
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

### **Schematics, pcb layouts,  gerbers **
of YAKS2-TITUO are open source, released under the Creative Commons CC BY-NC license.
This means that you are free to:

|                      |                                                                        |
| -------------------- | ---------------------------------------------------------------------- |
|      SHARE           |      copy and redistribute the material in any medium or format        |
|      ADAPT           |      remix, transform, and build upon the material                     |

      
Under the following terms:

|                       |                                                                        |
| --------------------- | ---------------------------------------------------------------------- |
|     Attribution       | You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use. |
|      NonCommercial    | You may not use the material for commercial purposes.                  |
|      ShareAlike       | If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.          |
| No additional restrict| You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.  |


### **YAKS2-TITUO FIRMWARE** 
is free to download, copy and redistribuite to be used in conjuction with any YAKS2-TITUO board.
The firmware **CANNOT** be in any way:
- used for any other purpose than YAKS2-TITUO (e.g. flashed in other boards)
- sold, rent or leased. If you were asked to pay for it, you've been tricked


## **Warranty Disclaimer and Limitation of Liability**

YAKS2-TITUO is an hobbyist project without any commercial intention; you understand that we cannot and do not guarantee or warrant neither the YAKS2-TITUO hardware (including but not limited to: schematics, gerbers, pcb, components, assembling, etc.) nor the YAKS2-TITUO software (firmware, etc) from defects, breakage or loss of functionality. You are using HID2AMI under your exclusive risk and responsibility; please understand and AGREE that **WE WILL NOT BE LIABLE FOR ANY LOSS OR DAMAGE CAUSED BY EITHER ANY USE OR ANY MISUSE OF YAKS2-TITUO**

BY MAKING USE OF YAKS2-TITUO, YOU EXPRESSLY AGREE THAT YOUR WILL ACCEPT IT ON "AS IS" BASIS WITHOUT ANY WARRANTIES OF ANY KIND, EITHER EXPRESS OR IMPLIED. YOU ALSO EXPRESSELY AGREE THAT YOUR USE OF HID2AMI HARDWARE AND ITS SOFTWARE COMPONENTS IS AT YOUR OWN RISK. NEITHER THE AUTHOR (Sampedenawa) NOR ANY PERSON ASSOCIATED WITH THE AUTHOR MAKES ANY WARRANTY OR REPRESENTATION WITH RESPECT TO THE COMPLETENESS, SECURITY, RELIABILITY, QUALITY, ACCURACY OR AVAILABILITY OF THE HID2AMI HARDWARE/SOFTWARE.

IF YOU DO NOT UNDERSTAND AND EXPRESSLY AGREE WHAT STATED ABOVE, YOU ARE NOT ENTITLED BY THE AUTHOR TO USE HID2AMI FOR ANY PURPOSE.
