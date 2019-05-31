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
- Kickstart selection by CTRL-A-A and RST methos (can be easily modded for AUTOSENSE - 1 wire mod)
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





### ASSEMBLING REFERENCE DOCS

At first, look at a fully assembled board (please note some vacancies: not all pads shall be populated)

[Reference Board: TOP](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Pics/HID2AMI.Black.Top.jpg "Reference Board: TOP")

[Reference Board: BOTTOM](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Pics/HID2AMI.Black.Bottom.jpg "Reference Board: BOTTOM")

#### **SCHEMATICS**

[HID2AMI v1.0.0 SCHEMATICS SHEET](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.0.0.redist.sch)

[HID2AMI v1.1.0 SCHEMATICS SHEET](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.1.0.redist.sch)

#### **REFERENCE LAYOUTS**

[Reference Layout v1.0.0 Top](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.0.0.redist.layout.top.pdf)

[Reference Layout v1.0.0 Bottom](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.0.0.redist.layout.bottom.pdf)

[Reference Layout v1.1.0 Top](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.1.0.layout.top.pdf)

[Reference Layout v1.1.0 Bottom](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.1.0.layout.bottom.pdf)

#### **BILL OF MATERIALS**

Components noted as "Optional" fulfil the general purpose STM32F1x reference design; generally speaking they can be safely omitted from the assembly of HID2AMI. Consider soldering any of them in case you experience some instability of any kind (never experienced so far).

LED1 is "run mode" indicator; it blinks at variable rates to indicate HID2AMI running status (suggesetd colors: green, yellow, white)
- When in BOOTLOADER mode, a fast blink means bootloader running and waiting for the "App" to be flashed/upgraded
- When in APP mode, a "regular" blinking means the App is running and waiting for input; a slower blinking (upon connecting a peripheral), means the peripheral correctly identified and mapped 

LED2 is the "power on" indicator; if lit then your board gets correct +5V and +3.3V power supply 

For both LED1 and LED2, the suggested value for their respective limiting current resistors is 10k, but you can safely experiment any value in range 1k-47k depending on the led components characteristics and light efficiency (and your personal taste)

[Reference BOM v1.0.0](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.0.0.BOM.txt)

[Reference BOM v1.1.0](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.1.0.BOM.txt)


### **GERBER FILES**

[HID2AMI v1.0.0 DELUXE GERBER FILES](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.0.0.redist_2019-01-19.zip)

[HID2AMI v1.1.0 DELUXE GERBER FILES](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.1.0.redist_2019-02-28.zip)

### **EAGLE SCHEMATICS AND BOARD LAYOUT**

[HID2AMI v1.0.0 DELUXE SCHEMATICS](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.0.0.redist.sch)

[HID2AMI v1.0.0 DELUXE BRD](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.0.0.redist.brd)

[HID2AMI v1.1.0 DELUXE SCHEMATICS](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.1.0.redist.sch)

[HID2AMI v1.1.0 DELUXE BRD](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Board/HID2AMI.Deluxe.Rev1.1.0.redist.brd)

### **BOOTLOADER**

Current BOOTLOADER version is 1.3.0. You can freely get it from here [HID2AMIBOOTLOADER](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Firmware/HID2AMIBOOTLOADER.dfu)


### **FLASHING INSTRUCTIONS**

Detailed flashing instructions, and how to get your personal HID2AMI board code, can be found here, for both Linux (courtesy by Sukkopera) and Windows:

[HID2AMI FLASHING INSTRUCTIONS](https://github.com/EmberHeavyIndustries/HID2AMI/blob/master/Docs/Flashing.Instructions.md)


## **LICENSE TERMS**
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

### **Schematics and pcb gerbers**
of HID2AMI are open source, released under the Creative Commons CC BY-NC license.
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


### **HID2AMI BOOTLOADER** 
is free to download, copy and redistribuite.

### **HID2AMI APP** 
is distribuited by request from the author; each instance is strictly tied 1:1 to a particular HID2AMI board. You are not allowed to copy and distribuite HID2AMI APP in any medium or format. 

## **DISTRIBUTION AND PRICING POLICY**
I've spent a great effort in designing and developing this app, so I would be grateful if you'd be happy to contibute to its future development. I decided to release all project's details, schematics and gerbers for free to everyone, but retaining myself close control over the firmware app. Being this one a no-profit hobbyist project, I can't guarantee any volume production of boards, so I will following the following distributio policies, for who may be interested in having one:

- Software only
  - You build the board yourself, by mean of the public gerbers or by a compatible custom layout you derive from schematics
  - You get the APP from me by sending me a request together with your personal 4-digits code (see instructiuons above how to get it)
  - Availability to serve request and cost of the app shall be exposed here or on the Amiga Forums I (Sampedenawa) am frequenting. Find HID2AMI on [Amigapage](http://www.amigapage.it), [EAB](https://eab.abime.net), [A1K](https://www.a1k.org). 

- DYI KIT
  - You build the board yourself by getting from me the pcb and all needed components
  - You get the APP from me by sending me a request together with your personal 4-digits code 
  - Availability and costs of DIY kits shall be exposed here or on the Amiga Forums I (Sampedenawa) am frequenting. Find HID2AMI on [Amigapage](http://www.amigapage.it), [EAB](https://eab.abime.net), [A1K](https://www.a1k.org).

- COMPLETE BOARD
  - You get the fully working board from me by sending me a request 
  - (Rare) Availability and costs of complete boards shall be exposed here or on the Amiga Forums I (Sampedenawa) am frequenting
. Find HID2AMI on [Amigapage](http://www.amigapage.it), [EAB](https://eab.abime.net), [A1K](https://www.a1k.org).

## **Warranty Disclaimer and Limitation of Liability**

HID2AMI is an hobbyist project without any commercial intention; you understand that we cannot and do not guarantee or warrant neither the HID2AMI hardware (including but not limited to: schematics, gerbers, pcb, components, assembling, etc.) nor the HID2AMI software (bootloader, app, etc) from defects, breakage or loss of functionality. You are using HID2AMI under your exclusive risk and responsibility; please understand and AGREE that **WE WILL NOT BE LIABLE FOR ANY LOSS OR DAMAGE CAUSED BY EITHER ANY USE OR ANY MISUSE OF HID2AMI**

BY MAKING USE OF HID2AMI, YOU EXPRESSLY AGREE THAT YOUR WILL ACCEPT IT ON "AS IS" BASIS WITHOUT ANY WARRANTIES OF ANY KIND, EITHER EXPRESS OR IMPLIED. YOU ALSO EXPRESSELY AGREE THAT YOUR USE OF HID2AMI HARDWARE AND ITS SOFTWARE COMPONENTS IS AT YOUR OWN RISK. NEITHER THE AUTHOR (Sampedenawa) NOR ANY PERSON ASSOCIATED WITH THE AUTHOR MAKES ANY WARRANTY OR REPRESENTATION WITH RESPECT TO THE COMPLETENESS, SECURITY, RELIABILITY, QUALITY, ACCURACY OR AVAILABILITY OF THE HID2AMI HARDWARE/SOFTWARE.

IF YOU DO NOT UNDERSTAND AND EXPRESSLY AGREE WHAT STATED ABOVE, YOU ARE NOT ENTITLED BY THE AUTHOR TO USE HID2AMI FOR ANY PURPOSE.
