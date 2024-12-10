# Project  Cirrus Logic 542x ISA video card
Remaking from Cirrus Logic Databook  "CL-GD542X_Technical_Reference_Manual_Jan1994"
![grafik](https://github.com/user-attachments/assets/78f533ff-fe82-43f0-a3d6-b032cc464d83)

# PCB Revision History 
- 542xISA-000 initial draft
- 542xISA-001 few minor bug fixing (IOCS16/MEMCS16 swap, added output filter)
- 542xISA-002 change of XTAL Footprint to HC-49  (not tested, only change of layout is  XTAL-footprint)

# Feartures
- Cirrus Logic (CL-GD5422-5429) video chipset (5420 is not recommend for this design)
- good chocie video card for ISA bus platform
- up to 2 MB DRAM
- 80 MHz integrated RAMDAC (GD5429: 86 MHz )
- Win 3.1, Win9x, Win NT 3.51 & 4 driver available
- cheap GD542x VLB card as compoment donor.
- cheap 2 layer platine layout 
  
# Issues 
- some 542x chip has vertical noise/stripe on TFT. (It is not pcb issuses)


# notes
- GD5420/22/24 support only 1 MB DRAM
- U11 & U12  is first 1 MB , U13/14 is seconds MB (except 5420, only U12 and U14 )
- all component with  followed ID is config strap (R55, R57, R59, R61, R63, R69, R73)
- SPI-EEPROM is optional.

 

# Bill of material

- [![csv-file 001 ](https://github.com/matt1187/542x_ISA/blob/main/Gerber/542xISA_001.csv)]
- [![csv-file 002(not tested)](https://github.com/matt1187/542x_ISA/blob/main/Gerber/542xISA-002.csv)]
- [Config strap (R55, R57, R59, R61, R63, R69, R73) Place all resistor except R69
- [![Gerber file 001](https://github.com/matt1187/542x_ISA/blob/main/Gerber/542xISA-001.zip]]
- [![Gerber file 002(not tested)](https://github.com/matt1187/542x_ISA/blob/main/Gerber/542xISA-002.zip)]

# driver & ROM 
- [![Cirrus Logic ROM generic for all GD542x, from VLB donor card](https://github.com/matt1187/542x_ISA/blob/main/ROM/cirrus5428.zip)]





# License
The project is free for non-commercial reproduction. Do not sell it on Ebay or other platforms for profit. Do not make a closed source derivative. Share your experiences and ideas with the community.

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
