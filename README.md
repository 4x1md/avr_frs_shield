# AVR Fuse Rescue Shield for Arduino Uno
AVR Fuse Rescue Shield based on [Arduino-based AVR High Voltage Programmer](http://mightyohm.com/blog/2008/09/arduino-based-avr-high-voltage-programmer/) by Jeff Keyzer W6OHM aka [@mightyohm](https://twitter.com/mightyohm).

## Overview
While working on a new prototype for my [GPS module for Yaesu VX-8DR/DE transceivers](https://github.com/4z7dtf/vx8_gps), I made some newbie errors burning incorrect fuses into the ATmega328P microcontroller and bricked them. After some research I found [MightyOhm's High Voltage Programmer](http://mightyohm.com/blog/2008/09/arduino-based-avr-high-voltage-programmer/) which could bring them back to life. His programmer was designed as Arduino shield thus I could use the Arduino Uno board I already had. In my project I used MightOhm's schematics with minor changes and his Arduino code as is.

## Sechematics
The schematics are almost the same as the original MightyOhm's. Two minor changes are:

1. Zener diode for getting 12V from unregulated power supply.
2. A led connected to microcontrollers Vcc line.

![AVR Fuse Rescue Shield Schematics](https://raw.githubusercontent.com/4z7dtf/avr_frs_shield/master/images/schematic.png)

## PCB Design
The PCB was designed using KiCAD software. As it was meant to be produced at home I designed it as single layer board. There are some front side tracks in the design which were replaced by jumper wires in the real PCB. Toner Transfer method was used to transfer the drawings to copper and front side.

![AVR Fuse Rescue Shield Schematics](https://raw.githubusercontent.com/4z7dtf/avr_frs_shield/master/images/pcb_color.png)

### Copper side
Print version: [avr_frs-pcb.pdf](https://github.com/4z7dtf/avr_frs_shield/blob/master/printable/avr_frs-pcb.pdf)

![AVR Fuse Rescue Shield Schematics](https://raw.githubusercontent.com/4z7dtf/avr_frs_shield/master/images/pcb_bw.png)

### Silk screen
Print version: [avr_frs-silk.pdf](https://github.com/4z7dtf/avr_frs_shield/blob/master/printable/avr_frs-silk.pdf)

![AVR Fuse Rescue Shield Schematics](https://raw.githubusercontent.com/4z7dtf/avr_frs_shield/master/images/pcb_silk.png)

## Software


To be completed...

## Photos

![]()




## Sources
1. []()
2. 

## Questions? Suggestions?
You are more than welcome to contact me with any questions, suggestions or propositions regarding this project. You can:

1. Visit [my QRZ.COM page](https://www.qrz.com/db/4Z7DTF)
2. Visit [my Facebook profile](https://www.facebook.com/Dima.Meln)
3. Write me an email to iosaaris =at= gmail dot com
