[![hacs_badge](https://img.shields.io/badge/HACS-Default-41BDF5.svg?style=for-the-badge)](https://github.com/hacs/integration)

# Victron Instant Readout Integration (JP)

_This is forked from https://github.com/keshavdv/victron-hacs just for the purpose of working around some issues with BLE updates._

_This fork will go away once https://github.com/keshavdv/victron-hacs/issues/123, https://github.com/keshavdv/victron-hacs/issues/99 etc are fixed._

_Unless you currently have issues getting data, you are probably better off using the plugin from that repo_

This integration allows exposing data from Victron devices with Instant Readout enabled in Home Assistant.

Supported Devices & Entities:

- SmartShunt 500A/500mv and BMV-712/702 provide the following data:
  - Voltage
  - Alarm status
  - Current
  - Remaining time (mins)
  - State of charge (%)
  - Consumed amp hours
  - Auxilary input mode and value (temperature, midpoint voltage, or starter battery voltage)
- Smart Battery Sense
  - Voltage
  - Temperature (°C)
- MPPT/Solar Charger
  - Charger State (Off, Bulk, Absorption, Float)
  - Battery Voltage (V)
  - Battery Charging Current (A)
  - Solar Power (W)
  - Yield Today (Wh)
  - External Device Load (A)

# Installation

## Manual

1. Clone the repository to your machine and copy the contents of custom_components/ to your config directory
2. Restart Home Assistant
3. Setup integration via the integration page.

## HACS

1. Add the integration through this link:
   [![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=jamezpolley&repository=victron-hacs&category=integration)
2. Restart Home Assistant
3. Setup integration via the integration page.
