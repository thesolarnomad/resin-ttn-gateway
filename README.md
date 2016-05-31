# Resin.io The Things Network Gateway based on Raspberry Pi

This uses the [Single Channel LoRaWAN Gateway](https://github.com/tftelkamp/single_chan_pkt_fwd) on a Raspberry Pi [as described by Dragino](http://www.instructables.com/id/Use-Lora-Shield-and-RPi-to-Build-a-LoRaWAN-Gateway/) on [resin.io](http://resin.io).

It uses a Raspberry Pi Model B+ V1.2 and an [Modtronix inAir9](http://modtronix.com/inair9.html) SX1276 LoRa Module.

## Default pin mapping:

| SX1276 | Raspberry Pi |
|--------|--------------|
| 3.3V   | pin #1       |
| GND    | pin #6       |
| MISO   | pin #21      |
| MOSI   | pin #19      |
| SCK    | pin #23      |
| NSS    | pin #22      |
| DIO0   | pin #7       |
| RST    | pin #11      |

## Environment variables for resin.io

| Variable name | Value                                                                                 | More info                              |
|---------------|---------------------------------------------------------------------------------------|----------------------------------------|
| DIO_PIN       | 7                                                                                     | Optional. Defaults to 7.               |
| RST_PIN       | 0                                                                                     | Optional. Defaults to 0.               |
| SS_PIN        | 6                                                                                     | Optional. Defaults to 6.               |
| EMAIL_ADDRESS | you@domain.com                                                                        | Optional, empty by default.            |
| FREQUENCY     | [Depends on your location and chip](https://github.com/TheThingsNetwork/gateway-conf) | Optional. In Hz. Defaults to 868100000 |
| HOSTS         | [Depends on your location](https://github.com/TheThingsNetwork/gateway-conf)          | Optional                               |
| LATITUDE      | [Your latitude](http://www.gps-coordinates.net/)                                      | Optional. Float. Defaults to 0.0       |
| LONGITUDE     | [Your longitude](http://www.gps-coordinates.net/)                                     | Optional. Float. Defaults to 0.0       |
| ALTITUDE      | [Your altitude](http://www.gps-coordinates.net/)                                      | Optional. Integer. Defaults to 0       |
