# DA CLOCK

This repository contains the schematics and board layouts for Eagle of the different DaClock versions I've done so far.
The common parts between all these versions are: a microcontroller on board with some power management, an RTC and connectors for LED strips or matrices.

Current version is 3.0, based on ESP8266 and DS1337S, also features a buzzer and support for both WS2812 strips/matrices and 5050 "single color" strips.

## Versions

### Version 1.2

![DaClock 1.2 - schema](/images/daclock-1.2-schema.png)


![DaClock 1.2 - layout](/images/daclock-1.2-layout.png)


### Version 2.1 - WIFI

![DaClock 2.1 - schema](/images/daclock-2.1-schema.png)


![DaClock 2.1 - layout](/images/daclock-2.1-layout.png)


### Version 3.0 - WIFI LITE

This is the latest version of the DA CLOCK board, a custom ESP8266-based clock with an RTC, a buzzer and output to handle WS2812 strips.

![DaClock 3.0 - schema](/images/daclock-3.0-schema.png)


![DaClock 3.0 - layout](/images/daclock-3.0-layout.png)

#### Bill of materials for a WS2812-based clock

|Item|Buy|Quantity|CPU <sup>units</sup>|Total|
|---|---|---|---|---|---|---|
|Tinkerman Da Clock WIFI 3.0|[OSH Park](https://oshpark.com/shared_projects/gDLQyM9I)|1|6.57€ <sup>3</sup>|6.57€|
|Ai-Thinker ESP12F|[Aliexpress](http://s.click.aliexpress.com/e/mUZjemI) / [Ebay](https://rover.ebay.com/rover/1/711-53200-19255-0/1?icep_id=114&ipn=icep&toolid=20004&campid=5338044841&mpre=http%3A%2F%2Fwww.ebay.com%2Fitm%2FESP8266-Remote-Serial-Port-WIFI-Transceiver-Wireless-Module-Esp-12F-AP-STA-%2F272408386985%3Fhash%3Ditem3f6cce1da9%3Ag%3ArywAAOSwZJBX-7RV)|1|2.10€ <sup>5</sup>|2.10€|
|AMS1117-3.3|[Aliexpress](http://s.click.aliexpress.com/e/uj6iuNv) / [Ebay](https://rover.ebay.com/rover/1/711-53200-19255-0/1?icep_id=114&ipn=icep&toolid=20004&campid=5338044841&mpre=http%3A%2F%2Fwww.ebay.com%2Fitm%2FNew-10pcs-AMS1117-LM1117-3-3V-1A-SOT-223-Voltage-Regulator-NT00206-Ship-Today-%2F112049991237%3Fhash%3Ditem1a16b32e45%3Ag%3AqV8AAOSw14xWNwXc)|1|0.03€ <sup>50</sup>|0.03€|
|1N4148 SMD Diode|[Aliexpress](http://s.click.aliexpress.com/e/i2nayrB)|1|0.04€ <sup>100</sup>|0.04€|
|Buzzer|[Aliexpress](http://s.click.aliexpress.com/e/VbeAu3z) / [Ebay](https://rover.ebay.com/rover/1/711-53200-19255-0/1?icep_id=114&ipn=icep&toolid=20004&campid=5338044841&mpre=http%3A%2F%2Fwww.ebay.com%2Fitm%2FNew-10pcs-5v-Active-Buzzer-Continous-Beep-High-quality-The-sound-Alarm-HT00202-%2F281280117872)|1|0.15€<sup>10</sup>|0.15€|
|S8550 SMD NPN transistor|[Aliexpress](http://s.click.aliexpress.com/e/VZ3FYN7)|2|0.02€<sup>100</sup>|0.04€|
|100nF 0805 ceramic capacitor||1|0.01€ <sup>100</sup>|0.01€|
|1uF 10V 0805 tantalum capacitor|[Aliexpress](http://s.click.aliexpress.com/e/ey3ZVn2)|2|0.06€ <sup>50</sup>|0.12€|
|1000uF 16V electrolytic SMD capacitor|[Aliexpress](http://s.click.aliexpress.com/e/MjQ7eMf)|1|0.19€ <sup>10</sup>|0.19€|
|200Ohm 0805 resistor||1|0.01€ <sup>100</sup>|0.01€|
|10KOhm 0805 resistor||7|0.01€ <sup>100</sup>|0.07€|
|2 positions 5mm screw terminal|[Aliexpress](http://s.click.aliexpress.com/e/a2fqnM7)|1|0.06€ <sup>100</sup>|0.06€|
|3 positions 5mm screw terminal|[Aliexpress](http://s.click.aliexpress.com/e/Vjaa2RB)|1|0.07€ <sup>100</sup>|0.07€|
|3 position male header||1|0.01€ <sup>100</sup>|0.01€|
|5 position male header||1|0.01€ <sup>100</sup>|0.01€|
|Jumper||1|0.01€ <sup>100</sup>|0.01€|
|**Total**||||9.49€|

* (units) Minimum quantity for the stated price.
* Prices are based on the cheapest option, usually Aliexpress.
* Check the schematic (image or eagle file) for relation between parts and values.

## Firmware

* Project [Wordclock](https://bitbucket.org/xoseperez/wordclock) uses version 1.0 of this board (atmega328p based).
- Project [Slices](http://github.com/xoseperez/slices) uses version 3.0 of this board (ESP8266 based).

## Open Hardware

Hardware designs (schematics and CAD) files are licensed under the [Creative Commons Attribution-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-sa/3.0/) and follow the terms of the [OSHW (Open-source hardware) Statement of Principles 1.0.](http://freedomdefined.org/OSHW)
