# gba-cartridge

The aim of this repository is to reverse engineer a chinese produced GBA reproduction cartridge.
The cartridge of interest was bought on [Aliexpress over here](https://de.aliexpress.com/item/1005005879617919.html).


## Front
![pinout](docs/pinout_front.png)

## Back
![pinout](docs/pinout_back.png)

# Hardware 

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



