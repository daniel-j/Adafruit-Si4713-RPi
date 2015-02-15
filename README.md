# Python class for connecting to the Adafruit Si4713 (FM transmitter) breakout-board

Code reused from Adafruit's example code and Hansipete's original code. Converted into a reusable class by djazz/daniel-j. Uses Adafruit_I2C and RPi.GPIO, make sure those are available!

Original code is from this Adafruit forums thread:
https://forums.adafruit.com/viewtopic.php?f=50&t=58453

This file is included in this repo:
https://github.com/adafruit/Adafruit-Raspberry-Pi-Python-Code/blob/master/Adafruit_I2C/Adafruit_I2C.py

Don't forget to enable I2C! If you're on Raspbian, use `sudo raspi-config` and enable it.

## How to use

Connect the board's I2C pins to the RPi I2C pins and the reset pin to GPIO4 (right next to the I2C/SPI pins). You can use 5V or 3V3 to power the board. Connect an audio source to the transmitter. Start the example code with `sudo python2 radio.py`. Tune in to 101.0 MHz, and you should hear whatever audio you're inputting to the board. You should (if you have an RDS/RBDS supporting FM radio) see the station title too!

Happy pi-casting!