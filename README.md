# EcoFlow BLE

[![hacs_badge](https://img.shields.io/badge/HACS-Default-41BDF5.svg)](https://github.com/hacs/integration)
[![Validation hassfest](https://github.com/rabits/ha-ef-ble/actions/workflows/validate-hassfest.yaml/badge.svg)](https://github.com/rabits/ha-ef-ble/actions/workflows/validate-hassfest.yaml)
[![Validation HACS](https://github.com/rabits/ha-ef-ble/actions/workflows/validate-hacs.yaml/badge.svg)](https://github.com/rabits/ha-ef-ble/actions/workflows/validate-hacs.yaml)

Unofficial EcoFlow BLE devices Home Assistant integration will allow you to communicate with a
number of EcoFlow devices through bluetooth and monitor their status / control parameters.

Recognized devices:
* Smart Home Panel 2 (EF-HD3####, FW Version: 4.0.0.122, WiFi Version: 2.0.1.20)
* Delta Pro Ultra (EF-YJ####, FW Version: 5.0.0.25, WiFi Version: 2.0.2.4)
* River 3, River 3 Plus (EF-R3####, FW Version: 1.0.0.0)
* Delta 3 Plus (EF-D3####, FW Version: 6.49.74.44)

**NOTICE**: this integration utilizes Bluetooth LE of the EF device, which is supporting just one
connection at a time - so if you want to manage the device through BLE from your phone, you will
need to disable this device in HA for that and later re-enable it to continue to collect data. It's
an internal EF device limitation, so not much to do here...

## WARNING: Support & Warranty

Sorry, limited support and no warranty - you on your own and I take no responsibility for any of
your actions. We all grown-ups here and know that we deal with quite dangerous voltages and storage
devices that could injure or cause death. So make sure you know what you doing for each and every
step - otherwise you can't use the provided information in this repository or integration.

In case you see some issues with your device after using this integration - ecoflow support could
be unable to help you. Author of the integration is not connected to EcoFlow anyhow and they can't
support anything you will find here.

## Usage

Install the integration as custom_component and it will automatically find the supported devices.
It will also require your user id that was created during initialization of your device with app.

Please refer to the wiki page to find more info: https://github.com/rabits/ha-ef-ble/wiki

## Development & Reverse

Information about how that was reversed you can find here: https://github.com/rabits/ef-ble-reverse

If you want to help with this integration - your changes will be most welcomed, but I recommend to
create a ticket first to discuss the needed features or upcoming changes to make sure they fit the
purpose of the integration.

## Legal

This repository is not for sale.

The work was done in order to localize devices and make them available / controllable in disaster
situations (unavailability of internet or cut-off the ecoflow servers). The official application
allows to connect via bluetooth, but to do that you have to login to the server. No server is here
and you screwed.

The requests to ecoflow usually ends up in support department and generally ignored, so there is no
way to get support from them. That gave me right to take it in my own hands and use my knowledge &
time to make my own way. There is no intention to harm any people anyhow - just to make sure you
will be safe in emergency situation, which is critical for such a product.
