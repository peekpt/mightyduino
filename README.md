## Mightyduino
A DIY Arduino type hardware board based on ATmega644p Atmega1284p

This project is free and based on @MCUDude's [MightyCore](https://github.com/MCUdude/MightyCore) which has awesome well designed kits for serious development with AVR's.
![top](https://github.com/peekpt/mightyduino/raw/master/img/3dtop.png)

Mightyduino is an Arduino with more memory than an Arduino Pro mini. It can use 644p (64k) or 1284p (128k) chips. Its voltage can be configured by U1 and the frequecy can be configured by the Murata's ressonator (crystal).
It has a power led and another one connected to pin D0. The push button performs reset. DTR pin can be used to external reset. The RAW pin is the input voltage **<16v**. The VCC pin is the regulator output and IC voltage, it can be loaded up to peak of **500mA**.

To burn the **bootloader** (optiboot 6.0) you must first install the [MightyCore boards](https://github.com/MCUdude/MightyCore#how-to-install) on Arduino App  , connect the ICSP pins to your bootloader programming hardware (eg. USBASP), select one of MCUDude's board that meet the specs you use and burn bootloader.
Then you can access (ttl-serial dongle) like a normal arduino on the serial pins (like arduino pro mini). Mightyduino uses the 'standard' pin mapping.


###Version History
- v1.3 - Changed C1 C3 footprint, add reset pin for SPI programming.
- v1.2 - Switch U1 shutdown pin 3 voltage to RAW
- v1.1 - Switched Led from pin D13 to D0, cosmetic improvements
- v1.0 - Initial release


###Quick Links:

Order boards from [OSHPark]
(https://oshpark.com/shared_projects/zuZ4OIae)

Or download the [Gerber files](https://github.com/peekpt/mightyduino/raw/master/gerber/gerbers.zip) for other pcb maker

Download the schematic [PDF](https://github.com/peekpt/mightyduino/blob/master/schematic.pdf)

ATmega datasheet [644p](http://www.atmel.com/images/doc2593.pdf) [1284p](http://www.atmel.com/images/doc8059.pdf)


## Screenshots

###Components
![Pin Map](https://github.com/peekpt/mightyduino/raw/master/img/components.png)
### Top
![top](https://github.com/peekpt/mightyduino/raw/master/img/3dtop.png)
### Bottom
![bottom](https://github.com/peekpt/mightyduino/raw/master/img/3dbottom.png)
###Pin Mapping
![Pin Map](https://github.com/peekpt/mightyduino/raw/master/img/atmega644p_standard_mapping.png)






