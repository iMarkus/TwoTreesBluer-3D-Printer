# TwoTreesBluer-3D-Printer

Documentation, firmware and set of utilities for my own use and personal needs. Don't blame me if it does not work or causes any other harm.

## Machine Specs
| Parameter | Value |
|--|--|
Number of nozzles|1|
Construction volume|235mm * 235mm * 280mm|
Printing method|SD-Card / online printing (by Serial UART communication through printer USB connector and some internet interface)|
IHM|3.5 inch color touch screen|
Machine speed|10~300mm/s|
Print speed|20~200mm/s|
Extrusion head temperature (highest)|260 °C|
Maximum hot bed temperature (highest)|100 °C|
Printing platform|Warm bed|
XY axis positioning accuracy|0.01mm|
Z axis positioning accuracy|0.004mm|
Recommended printed material|PLA, ABS and PETG|
Consumable filament diameter|1.75mm|
Print file format|G-Code|
Machine size|L=410mm * W=400mm * H=520mm|
Machine weight|7.5kg|
Power supply|127V~220V/240W|
Microcontroller|[STM32F103VET6 datasheet](https://github.com/TiagoPaulaSilva/Two-Trees-Bluer-3D-Printer/blob/master/Hardware/Motherboard/2.%20Datasheets/MCU/STM32F103VET6.pdf)|
Motor Driver|[TMC2209 datasheet](https://github.com/TiagoPaulaSilva/Two-Trees-Bluer-3D-Printer/blob/master/Hardware/Motherboard/2.%20Datasheets/Stepper%20Motor%20Driver/TMC2209.pdf)|
Stepper Motor|[US-17HS4401S datasheet](https://github.com/TiagoPaulaSilva/Two-Trees-Bluer-3D-Printer/blob/master/Hardware/Stepper%20Motors/US-17HS4401S.pdf)|
Motherboard|[MKS Robin Nano v1.2 schematic](https://github.com/TiagoPaulaSilva/Two-Trees-Bluer-3D-Printer/blob/master/Hardware/Motherboard/1.%20Schematic/MKS%20Robin%20Nano%20v1.2.pdf) ([source HW + FW](https://github.com/makerbase-mks/MKS-Robin-Nano-V1.X))|
Display|MKS Robin TFT35(FSMC) (schematic not available)|

More information on the manufacturer's official website: https://twotrees3d.com/

## Flashing

MKS Robin Nano V1.2, 28KB bootloader

Copy *.bin klipper firmware to SD card, rename it to Robin_Nano35.bin and insert into board.
Reset or re-power the board and update firmware.

Note that Robin Nano v1.2 needs to have TFT attached in order to flash, as work around you can rename bin file instead of Robin_Nano35.bin to Robin_Nano43.bin and it should flash without TFT.

## Display
Stock MKS TFT35 wont work with Klipper. 
There is a work around to use the display without touch (NoTouchScreenFirmware) - Untested

## References
<ul>
<li>https://www.klipper3d.org</li>
<li>https://www.klipper3d.org/Installation.html</li>
<li>https://github.com/TiagoPaulaSilva/Two-Trees-Bluer-3D-Printer</li>
<li>https://www.thingiverse.com/thing:5159319</li>
<li>https://github.com/teeminus/NoTouchScreenFirmware</li>
</ul>
