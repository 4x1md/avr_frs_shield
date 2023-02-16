# AVR Fuse Rescue Shield for Arduino Uno
AVR Fuse Rescue Shield based on [Arduino-based AVR High Voltage Programmer](http://mightyohm.com/blog/2008/09/arduino-based-avr-high-voltage-programmer/) by Jeff Keyzer W6OHM aka [@mightyohm](https://twitter.com/mightyohm).

## Overview
While working on a new prototype for my [GPS module for Yaesu VX-8DR/DE transceivers](https://github.com/4x1md/vx8_gps), I made some newbie errors burning incorrect fuses into ATmega328P microcontrollers and bricked them. After some research I found [MightyOhm's High Voltage Programmer](http://mightyohm.com/blog/2008/09/arduino-based-avr-high-voltage-programmer/) which could bring them back to life. His programmer was designed as Arduino shield thus I could use the Arduino Uno board I already had. In my project I used MightOhm's schematics with minor changes and his Arduino code as is.

I made this device for recovering ATmega328P chips. It may be compatible with other ATmega's, but you have to check the compatibility before you try. This shield uses high voltage which may damage your microcontroller.

## Schematics
The schematics are almost the same as the original MightyOhm's. Two minor changes are:

1. Zener diode for getting 12V from unregulated power supply.
2. A led connected to microcontrollers Vcc line.

The shield requires external power supply of 12 to 16V. Unregulated power source will work fine.

![AVR Fuse Rescue Shield Schematics](https://raw.githubusercontent.com/4x1md/avr_frs_shield/master/images/schematic.png)

## PCB Design
The PCB was designed using KiCAD software. As it was meant to be produced at home I designed it as single layer board. There are some front side tracks in the design which were replaced by jumper wires in the real PCB. Toner Transfer method was used to transfer the drawings to copper and front side.

![AVR Fuse Rescue Shield Schematics](https://raw.githubusercontent.com/4x1md/avr_frs_shield/master/images/pcb_color.png)

![AVR Fuse Rescue Shield Schematics](https://raw.githubusercontent.com/4x1md/avr_frs_shield/master/images/3d_pcb_0.png)

![AVR Fuse Rescue Shield Schematics](https://raw.githubusercontent.com/4x1md/avr_frs_shield/master/images/3d_pcb_1.png)

### Copper side
Print version: [avr_frs_pcb.pdf](https://github.com/4x1md/avr_frs_shield/blob/master/printable/avr_frs_pcb.pdf)

![AVR Fuse Rescue Shield Schematics](https://raw.githubusercontent.com/4x1md/avr_frs_shield/master/images/pcb_bw.png)

### Silk screen
Print version: [avr_frs-silk.pdf](https://github.com/4x1md/avr_frs_shield/blob/master/printable/avr_frs-silk.pdf)

![AVR Fuse Rescue Shield Schematics](https://raw.githubusercontent.com/4x1md/avr_frs_shield/master/images/pcb_silk.png)

## Software
MightyOhm's original [Arduino code](https://github.com/4x1md/avr_frs_shield/tree/master/avr_frs_arduino) is used without any modifications.

## Alignment
Correctly assembled device requires no alignment.

## How To Use The Device

1. Upload the code to Arduino Uno or compatible board.
2. Connect the shield to the the Arduino.
3. Connect power sources to the Arduino board and to the shield. The red led will light and the green will not.
4. Place the device to recover in the dedicated socket.
5. Press the button on the shield. The green led will light and the red will turn off.
6. Wait until the leds return to their previous states.
7. Enjoy your unbricked microcontroller!

## Photos

![AVR Fuse Rescue Shield](https://raw.githubusercontent.com/4x1md/avr_frs_shield/master/images/avr_frs_pcb.jpg)

![AVR Fuse Rescue Shield](https://raw.githubusercontent.com/4x1md/avr_frs_shield/master/images/avr_frs_silk.jpg)

![AVR Fuse Rescue Shield](https://raw.githubusercontent.com/4x1md/avr_frs_shield/master/images/avr_frs_top.jpg)

![AVR Fuse Rescue Shield](https://raw.githubusercontent.com/4x1md/avr_frs_shield/master/images/avr_frs_shield.jpg)

## Sources
1. [Arduino-based AVR High Voltage Programmer](http://mightyohm.com/blog/2008/09/arduino-based-avr-high-voltage-programmer/)
2. [Jeff Keller aka @mightyohm's Twitter](https://twitter.com/mightyohm)
3. [Atmel ATmega328P datasheet](http://www.atmel.com/images/atmel-8271-8-bit-avr-microcontroller-atmega48a-48pa-88a-88pa-168a-168pa-328-328p_datasheet_complete.pdf)

## Questions? Suggestions?
You are more than welcome to contact me with any questions, suggestions or propositions regarding this project. You can:

1. Visit [my QRZ.COM page](https://www.qrz.com/db/4X1MD)
2. Visit [my Facebook profile](https://www.facebook.com/Dima.Meln)
3. Write me an email to iosaaris =at= gmail dot com

## How To Say Thanks

If you like this project, or found here some useful information and want to say thanks, or encourage me to do more, you can buy me a coffee!

<a href="https://www.buymeacoffee.com/4x1md" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>

73 de 4X1MD
