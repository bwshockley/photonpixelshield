Photon Pixel Shield
========
The photon pixel shield is a small board for interfacing between a [particle.io](https://www.particle.io/) photon and some WS8212 based LED strips.  Specifically, this board was made to drive [Neopixel](https://www.adafruit.com/category/168) strips.

Power Requirements
--------
The board takes in 5V only - up to 1A - and is used to power the photon and the pixel strip.  Please note that current requirements are mostly driven by the number of LEDs being driven.  Each WS8212 LED uses a maximum of 20mA, which can add up quickly.  As such, at 1A, it is recommended to power at most 50 LEDs with this.

Digital Control
--------
The WS8212 based LED strips can be controlled via the photon and the [Neopixel library](https://github.com/technobly/SparkCore-NeoPixel) from Adafruit built by technobly.  No digital pin is selected by default on the board.  Pin D2 is the default in the library.  To use the default connect the solder jumper for D2 on the back of the board.  Otherwise, you may select almost any digital pin in both software on through the jumper on the board.

BOM
--------
The majority of the [BOM](http://www.mouser.com/ProjectManager/ProjectDetail.aspx?AccessID=84ec81cb7a), which as of 3/18/2016 can be found on mouser, is around $4.  A simple 3mm power LED is required if you wish to have a power indicator.  The resistor marked 330ohm on the board is for the LED.  Replace with an appropriate resistor value for an LED chosen.
