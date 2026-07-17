# ESPHome Bluetooth Proxies

This repo hosts YAML configurations for a curated selection of known, tested devices that can serve as Bluetooth proxies for Home Assistant.

If a device is not included here it may have a suitable configuration in the [ESPHome Device Configuration Repository](https://devices.esphome.io/).

We only add configurations for devices that we have tested in-house, are happy to recommend, and that are readily available for consumers to buy.

## Installation

Flash the firmware directly from your browser via USB using the web installer on the [ESPHome Projects page](https://esphome.io/projects/).

## Updates

Installed devices receive over-the-air updates through their firmware `update` entity, which checks the production channel manifest at `https://firmware.esphome.io/bluetooth-proxy/<device>/manifest.json`.

Releases are versioned using CalVer (`YY.M.N`) and published from this repository. Every published release is promoted to the beta channel first; releases that are not marked as a prerelease are also promoted to the production channel. To follow the beta channel, point the `update` component's `source` at `manifest-beta.json` instead of `manifest.json` in your device configuration.
