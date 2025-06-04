<h1 align="center">
  ESPHome-IR-Light
</h1>

<h4 align="center">An ESPHome Config for controlling an IR remote controllable light.</h4>

<p align="center"><img src="images/example-product.png" width=512 alt="Example Product"></p>

<p align="center"><img src="images/hass-device-controls.png" width=512 alt="Home Assistant Device controls"></p>

## Features

* [x] Based on [ESPHome][esphome]
* [x] Realtime transmission to Home Assistant
* [x] Emulation of State via ESPHome device (on/off, brightness, color temp)

## What you need

* An ESP8266, ESP32 or similar board
  * A power supply (preferably USB)
* An IR transmitter board
  <p><img src="images/ir-transmitter-board.png" width=128 alt="IR Transmitter Board"></p>

## Analyzing existing remote controls

Have a look at this excellent guide to find out the IR codes of your remote control: [Faking an IR remote control using ESPHome](https://community.home-assistant.io/t/faking-an-ir-remote-control-using-esphome/369071)

## Flashing the firmware

* Create a new ESPHome configuration YAML file
* Copy the contents of [esphome-ir-light.yaml](esphome-ir-light.yaml) into it
* Customize the basic device configuration (Board, WiFi, etc.) to your liking
* Flash it onto your ESP based board

## Connect to Home Assistant

Add the ESPHome device to Home Assistant via the "Integrations" page.
The sensors and buttons will automatically appear.

# Attributions

The setup to find out the IR codes was done using this very helpful thread on the Home Assistant forums: [Faking an IR remote control using ESPHome](https://community.home-assistant.io/t/faking-an-ir-remote-control-using-esphome/369071)

Many thanks to all the people who contributed to the [ESPHome][esphome] project.

# License

CC0 see [LICENSE](LICENSE)

[esphome]: https://esphome.io/