# gba-cartridge

The aim of this repository is to reverse engineer a chinese produced GBA reproduction cartridge.
The cartridge of interest was bought on [Aliexpress over here](https://de.aliexpress.com/item/1005005879617919.html).


## Front
![pinout](docs/pinout_front.png)

## Back
![pinout](docs/pinout_back.png)

# Components 

The cartridge is using a *JS28F128M29EWH* as a flash storage to store the game and *KM68U1000ELTGI-10L* as SRAM for the savegame. 


* 1x JS28F128M29EWH
* 1x KM68U1000ELTGI-10L
* 1x Unknown 60 pin COB (Chip on Board)
* 1x 0603 Zero Ohm Resistor
* 1x 0603 ??? uF Capacitor


**JS28F128M29EWH**
| name  | meaning
|-------|----------------------------------------------------------------------|
|    JS | 56-pin TSOP, 14mm x 20mm, lead-free, halogen-free, RoHS-compliant |
|   28F | Parallel NOR interface |
|   128 | 128Mbit = 16 Megabyte | 
| M29EW | Embedded Flash memory (3V core, page read) |
|     H | Highest block protected by VPP/WP#; uniform block |


## What was my approach?

1. Find out which components are on the PCB
2. Follow the traces
3. Remove the COB to find the pinout beneath
?. Create gerber files without the COB
?. ???
?. Make an own mapper to replace the COB
?. ???
?. Create gerber files including the own mapper
