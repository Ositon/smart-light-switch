# A Smart Light Switch using Bluetooth LE 

![Smart Light Switch](https://raw.githubusercontent.com/MakeBluetooth/smart-light-switch/master/light-switch.jpg)

One of the real problems with the current generation of smart light bulbs, is that the smarts are in the bulb.

While they have been held up as a massive Internet of Things success story possibly, in the longer term, this will be not turn out to be the case. Because light bulbs are something that you turn on, and off, from a switch in the wall.

You can make most smart light bulb systems unresponsive by using the wall switch. Effectively a smart light bulb replaces a thing we use every day, the light switch, but it does it poorly. Really we need to replace the switch, not the bulb.

## What is a smart switch?

A smart light switch not only lets you turn the light on, or off, using the switch itself but also remotely via Bluetooth LE. The switch should also know it's current status — in other words whether the bulb is on or off — and send out a notification over Bluetooth to subscribed applications when the switch is toggled to allow them to update their local status.

## What hardware will I need?

![Smart Light Switch](https://raw.githubusercontent.com/MakeBluetooth/smart-light-switch/master/ble-smart-switch.png)

We'll need the following hardware to build the light switch:

 * [Arduino Uno](http://www.makershed.com/products/arduino-uno-revision-3)
 * [Adafruit nRF8001 Bluefruit LE](https://www.adafruit.com/products/1697)
 * A breadboard
 * An LED
 * A 220Ω and a 10kΩ resistor
 * Jumper wires
 * A tactile button switch 
 
You can use also use a [PowerSwitch Tail](http://www.makershed.com/products/powerswitch-tail-ii) to control a real world lamp using your switch instead of a breadboarded LED.

![Switch with PowerSwitch Tail](https://raw.githubusercontent.com/MakeBluetooth/smart-light-switch/master/ble-light-with-powertail.png)

Since the PowerSwitch Tail needs to be pulled LOW to turn the mains powered device on, our code is identical to our LED example but with opposite logic for the pin controlling the Tail.