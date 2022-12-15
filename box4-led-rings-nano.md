# Box 4 - Addressable ("Pixel") LED Rings controlled by an Arduino Nano

## Overview
A more advanced style of LED lighting (but not hard to learn!), this Light Box uses LED rings made of addressable LED "pixels" that can each be individually programmed. Instead of using an "off-the-shelf" controller, this Light Box uses an Arduino Nano clone with C code that can control each LED. We are using a coding library called FastLED that does the hard work for us, and then using the DemoReel100 example code. This code is a great jumping-off-point to learning how to code for LEDs. This type of LEDs can also be controlled by an off-the-shelf controller that has standard patterns, or perhaps an advanced controller that has Wi-Fi or Bluetooth and app control.

## LED Specifications
* Addressable ("Pixels") = Yes
* Addressable Protocol = WS2812B
* Form Factor = Rings
* LED Spacing = (Not usual specified with rings of this type)
* Weather Rating = IP33 (Bare strip, not waterproof)
* Power Connector = USB (5v) into Arduino Nano
* Control = Arduino Nano with FastLED code

## Parts
* 8x32 256 Pixels LED matric ($20.29) - https://www.amazon.com/gp/product/B088BTXHRG/
* Arduino Nano clone ($17.49 for 3) - https://www.amazon.com/gp/product/B01DLIJQA2/
* JST SM 3 Pin connector. Connector is soldered to Nano, connects to LEDs ($9.49 for 20 pairs) - https://www.amazon.com/BTF-LIGHTING-Connectors-WS2812B-WS2811-WS2812/dp/B01DC0KIT2/
* Shadow Box ($37.98) - https://www.amazon.com/gp/product/B08BLHZ4FP

## Code
* The Arduino Nano is running the FastLED library "DemoReel100" example - https://github.com/FastLED/FastLED/blob/master/examples/DemoReel100/DemoReel100.ino (Once the FastLED Library is installed in the Arduino IDE, select Examples->FastLED->DemoReel100 and upload to the nano.
* We are using the default DATA_PIN which is (digital) pin D3
* The LED connector is connected to VIN (direct from USB, we don't want to run through the voltage regulator on the nano), GND, and D3


![LED product listing on Amazon](https://raw.githubusercontent.com/makerfx/light-boxes/main/images/box3-led-matrix.jpg)


![Arduino Nano clones product listing on Amazon](https://raw.githubusercontent.com/makerfx/light-boxes/main/images/arduino-nano-clones-amazon.jpg)



![JST SM Connector product listing on Amazon](https://raw.githubusercontent.com/makerfx/light-boxes/main/images/jst-sm-3pin-led-connectors.jpg)
