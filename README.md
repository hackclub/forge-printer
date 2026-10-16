## WIP Disclaimers

* This is an potential upcoming [Hack Club](https://hackclub.com) You Ship, We Ship (YSWS) program.

> **This project is semi-endorsed by Hack Club and isn't fully an official program yet.**

* Things are still under heavy development as the Forge Printer are WIP (Work in Progress) projects
* All information on this README is subject to change at any moment
* Submission requirements, images, and links are not final. Website URLs are placeholders and may not be functional
* If you have any questions about the Development of Forge (and are a teen under 18), feel free to visit [#forge-dev](https://hackclub.slack.com/archives/C078GBDKC03) on the [Hack Club Slack!](https://hackclub.com/arcade/?param=slack)

# Forge, Hack Club's 3D Printer

**[Landing Page](https://forge.hackclub.com)** | **[Gallery](https://forge.hackclub.com/gallery)**

2nd Place Finalist of the Hack Club Arcade Showcase 2024, out of over 2000 projects.

Find problems in the world and use programmatic 3D modeling to solve them. Submit your solutions to the Gallery and get a Forge 3D Printer
Forge is planned to be a **You Ship, We Ship** project from [Hack Club](https://hackclub.com).

Forge is **fully open source**. We encourage all to submit to the gallery through PRs! However, you must be a teenager or younger to receive a free printer.


## About the Forge Printer

The Forge Printer is a fast, inexpensive, and compact cantilevered 3D Printer. More details soon!

## Specifications

**These are Forge's specifications as of June 10, 2025. We're currently still in the process of building MK2. More details will be published soon.**

* STM32F405RGT6 32-Bit MCU
* TMC2209 Stepper Drivers
  * Reduced Motor Noise
  * Sensorless XY homing  
* TZ-E3 Hotend
  * 300°C Maximum Temperature
  * Designed around the Bambu Lab X1C hotend
  * 30mm³/s max flow rate
* 120x120x140mm Build Volume
  * Up to 100°C heated bed temperature
  * Magnetic Textured PEI Plate
* MGN9C Linear Rails
* ProtoXtruder Direct Drive Extruder (DDE)
* Fully Automatic Bed Leveling using BLTouch (ABL)
* Meanwell RPS-200-24 PSU (Integrated) with a protected C14 Inlet (used on the majority of consumer 3D printers)
* PLA, PETG, TPU capable
  * ABS and ASA are possible but require an enclosure and active ventilation
* Aluminum and 3D Printed ASA frame
* [DragonBurner](https://github.com/chirpy2605/voron/tree/main/V0/Dragon_Burner) Toolhead
* Up to 500mm/s Print Velocity*
   *This number is an estimate, real print speeds will be updated as Forge's development continues

## Firmware

* The Forge Mainboard will run on Marlin Firmware. (Custom, open source Forge Firmware had been planned but development has been halted as as of right now it is unrealistic)

* **The Forge Mainboard is supported by Klipper**
  * Using the Forge Printer with Klipper will be possible! The latest revision of the Forge Mainboard (2 layer PCB version) runs a STM32F405 which is fully compatible with Klipper! Additionally, we'll be providing a Klipper [WiP configuration file](https://github.com/hackclub/Forge/blob/main/Firmware/klipper) and OrcaSlicer profiles (Coming Soon) for you!
  * SBC Info:
    * **A Raspberry Pi Zero 2W will be required for *Klipper*. You can also use another SBC (that can run MainSailOS or Fluidd) with the same form factor. However, the Zero W (1st Gen) is highly not recommended due to performance limitations. Larger SBCs like the Raspberry Pi 1/2/3/4/5 boards are not compatible due to size limitations. We'll be providing a Raspberry Pi Zero Bracket available to print closer to MK2's launch!** The Forge Mainboard connects to the SBC via GPIO to GPIO, therefore, SPI touchscreens are not recommended.

## Additional notes

* The full Forge Printer and Mainboard BOM will soon be at the bottom of this doc. The Forge Printer BOM will not be available until we begin prototyping. However, the BOM for the Forge Mainboard is currently available as a CSV in `Electronics/Motherboard/billofmaterials.csv`.
* The estimated value of the Forge Printer is $200-$300, but this estimate will change over time (Additionally, tariffs may impact this cost in the future).
  * However, our goal is to offer Forge for free for teens 18 and under (details on how will come out soon) **
* Currently, Forge's parts and components are planned to be manufactured by [Siboor](https://www.siboor.com), a well-established supplier of 3D Printing components.
* Forge is designed in Onshape. [Check out the 3D model!](https://cad.onshape.com/documents/af44ce458991ef8deb280728/w/4e67c2ab8938e73dbc0acac0/e/91ca9a2c3befc6f76fb79dfa)

## Licensing

* **Currently, the Forge Project is GPLV3 (General Public License)**
* Anybody is allowed to freely use, advertise, modify, copy, or distribute any Forge designs or software as needed, with the condition that any public distribution or use of Forge software/design must also be open source and use GPL.
* For more information about this license, check out this [link](https://www.gnu.org/licenses/gpl-3.0.en.html)
  
## Support the Project!

* Forge's banking is fully transparent: [Check it out now!](https://hcb.hackclub.com/forge)
* [Donate to the Forge Project](https://hcb.hackclub.com/donations/start/forge), any dollar counts!
* **Forge is now offically [fiscally sponsored](https://en.wikipedia.org/wiki/Fiscal_sponsorship#:~:text=Fiscal%20sponsorship%20refers%20to%20the,and%20an%20established%20non-profit.) by Hack Club (a 501(c)(3) NPO with EIN 81-2908499)!

## Forge Project Credits:

### Forge Team:

* Krishna Meda (@EmperorNumerius) - Project Lead, Communications, Promotional Materials
* Arnnav Kudale (@blazecoding2009) - Project Lead, Sourcing, Electrical Engineering, Forge Firmware/Klipper Config Dev
* Evan Le (@lolwutboi987) - Design Engineering
* Michael Panait (@mikeymascatu) - Design Engineering, Promotional Materials
* Malav Patel (@astro-develops) - Design Engineer, Forge Landing Page Frontend Developer, Promotional Materials

Note that we all kind of work on everything, listed above is just what we generally do

### Special Thanks:

* Viv (@VivIsBee) - Forge Firmware Dev and PCB designer (MK1-MK2)
* Brendan Conover (@AGB556) - Former Design Engineer (MK2)
* Aaron Wong (@aaronw-dev) - Former Project Lead, Firmware Dev, Artist, Electrical Engineer (MK1)
* Engineering and Sales teams at [Siboor](https://www.siboor.com)
* [Polymaker](https://us.polymaker.com) for sponsoring $100 of filament!
* Patricio (@Patcybermind) - Former Forge Editor Developer
* Max Wofford (@maxwofford) - Hack Club HQ Representative, Forge Benefactor
* Alex Ren (@qcoral) - Thanks for the help with licensing!
* Jonathan Dong (@Dongathan-Jong) - Forge Art, Promotional Materials
* Beenana (@Beenana02) - Promotional Materials
* And the community for supporting this project!!

### Credits!
* [ProtoXtruder 2.0 by nhchiu](https://github.com/nhchiu/3DPrinter-Designs/tree/main/ProtoXtruder_2.0)
* [DragonBurner V8 Toolhead by chirpy2605](https://github.com/chirpy2605/voron/tree/main/V0/Dragon_Burner)
* [TZ-E3 2.0 DragonBurner Mount by cpp0xc0ffeeee](https://www.printables.com/model/1200549-tz-e3-20-mount-for-dragonburner-v8)
* [TZ E3 V2 Hotend CAD by Keram](https://www.printables.com/model/1051271-tz-e3-v2-hotend-bambulab-hotend-derivative-cad-wit)


