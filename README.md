![Logo](admin/sonoff.png)
# ioBroker Sonoff Adapter
==============

[![NPM version](http://img.shields.io/npm/v/iobroker.sonoff.svg)](https://www.npmjs.com/package/iobroker.sonoff)
[![Downloads](https://img.shields.io/npm/dm/iobroker.sonoff.svg)](https://www.npmjs.com/package/iobroker.sonoff)
[![Tests](https://travis-ci.org/ioBroker/ioBroker.sonoff.svg?branch=master)](https://travis-ci.org/ioBroker/ioBroker.sonoff)

[![NPM](https://nodei.co/npm/iobroker.sonoff.png?downloads=true)](https://nodei.co/npm/iobroker.sonoff/)

Requires node.js 4.0 or higher.

## Usage

This adapter communicates with Sonoff devices with Tasmota firmware or ESP devices via MQTT.

Following topics are expected:
- tele/DeviceNAME/STATE
- tele/DeviceNAME/SENSOR
- tele/DeviceNAME/INFOx
- tele/DeviceNAME/ENERGY
- cmnd/DeviceNAME/POWERx
- stat/DeviceNAME/POWERx
- /DeviceNAME/BM280/Temperature
- /DeviceNAME/BM280/Humidity
- /DeviceNAME/BM280/Temperatur
- /DeviceNAME/BM280/Feuchtigkeit
- /DeviceNAME/BM280/Vcc
- /DeviceNAME/BM280/VCC
- /DeviceNAME/BM280/Laufzeit
- /DeviceNAME/BM280/RSSI
- /DeviceNAME/BM280/POWER
- /DeviceNAME/BM280/POWER1
- /DeviceNAME/BM280/POWER2
- /DeviceNAME/BM280/POWER3
- /DeviceNAME/BM280/POWER4
- /DeviceNAME/BM280/Switch1
- /DeviceNAME/BM280/Switch2
- /DeviceNAME/BM280/Total
- /DeviceNAME/BM280/Today
- /DeviceNAME/BM280/heute
- /DeviceNAME/BM280/Yesterday
- /DeviceNAME/BM280/gestern
- /DeviceNAME/BM280/Faktor
- /DeviceNAME/BM280/Factor
- /DeviceNAME/BM280/Power
- /DeviceNAME/BM280/Leistung
- /DeviceNAME/BM280/Voltage
- /DeviceNAME/BM280/Spannung
- /DeviceNAME/BM280/Current
- /DeviceNAME/BM280/Strom
- /DeviceNAME/BM280/Punkt
- /DeviceNAME/BM280/Counter1
- /DeviceNAME/BM280/Counter2
- /DeviceNAME/BM280/Counter3
- /DeviceNAME/BM280/Counter4
- /DeviceNAME/BM280/Pressure
- /DeviceNAME/BM280/Druck
- /DeviceNAME/BM280/Approx. Altitude
- /DeviceNAME/BM280/Module
- /DeviceNAME/BM280/Version
- /DeviceNAME/BM280/Hostname
- /DeviceNAME/BM280/IPAddress
- /DeviceNAME/BM280/IPaddress
- /DeviceNAME/BM280/RestartReason
- /DeviceNAME/BM280/CarbonDioxide

**Note**: The list could be easily extended. Please send *Pull Requests* or *debug data* for unknown states to developer (via issue).

## Changelog

### 1.0.1 (2018-02-05)
* (bluefox) Ready for admin3
* (bluefox) Added CO2 sensor

### 1.0.0 (2017-11-27)
* (AlZiBa) typo @ alive
* (AlZiBa) add Todays power consumption for Sonoff POW
* (AlZiBa) unit of power consumption is kWh

### 0.3.3 (2017-11-03)
* (bluefox) Add counters

### 0.3.2 (2017-10-22)
* (Tan-DE) Small change for Switch1. Switch2 and additional IPaddress added.

### 0.3.1 (2017-10-12)
* (bluefox) Fix tests and LWT

### 0.3.0 (2017-10-06)
* (bluefox) Add INFO and ESP

### 0.2.0 (2017-10-05)
* (bluefox) Add ENERGY and DS18x20

### 0.1.0 (2017-10-01)
* (bluefox) initial commit

## License

The MIT License (MIT)

Copyright (c) 2017-2018, bluefox <dogafox@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
