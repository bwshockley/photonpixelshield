Photon Pixel Shield
Photon Pixel Shield
========
The photon pixel shield is a small board for interfacing between a [particle.io](https://www.particle.io/) photon and some WS2812 based LED strips.  Specifically, this board was made to drive [Neopixel](https://www.adafruit.com/category/168) strips.

Power Requirements - Diode and Fuse Sizing
--------
The board takes in 5V only  and is used to power the photon and the pixel strip.  Please note that current requirements are mostly driven by the number of LEDs being driven.  Each WS2812 LED uses an estimate of 20mA, which can add up quickly.

50   Neopixels: 1A
100 Neopixels: 2A

You will need to pick your own diode and fuse.  Since these devices are through hole, physical sizing isn't as much of a concern for finding the right part - mostly the current/voltage ratings.  I found fuses and diodes up to 3A easily fit.  Find a Diode with a low forward voltage (less than 0.5V)

_Note that v6 does away with the diode, so no need to pick or size that and v7 does away with both the diode and fuse._

Digital Control
--------
The WS2812 based LED strips can be controlled via the photon and the [Neopixel library](https://github.com/technobly/SparkCore-NeoPixel) from Adafruit built by technobly.  No digital pin is selected by default on the board.  Pin D2 is the default in the library.  To use the default connect the solder jumper for D2 on the back of the board.  Otherwise, you may select almost any digital pin in both software on through the jumper on the board.

BOM
--------
The majority of the [BOM](http://www.mouser.com/ProjectManager/ProjectDetail.aspx?AccessID=84ec81cb7a), which as of 12-JUL-18, can be found on Mouser.com for around $3.50.  You will need to pick a diode and re-settable fuse as noted above.

Power LED
--------
A simple 3mm power LED is required if you wish to have a power indicator.  The resistor marked RLED on the board is for the LED.  Populate with an appropriate resistor value for the LED chosen.  You can use [this calculate](http://ledcalc.com) for sizing the resistor.
