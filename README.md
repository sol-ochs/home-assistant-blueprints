# Home Assistant Blueprints for AWTRIX

A collection of Home Assistant automation blueprints for displaying data on Ulanzi/AWTRIX smart pixel clocks.

## Available Blueprints

### [Dexcom to AWTRIX Display](dexcom/)
Display real-time Dexcom glucose readings with trend arrows on your Ulanzi/AWTRIX clock.

## General Requirements

All blueprints require:
- [Home Assistant](https://www.home-assistant.io/) with MQTT configured
- [Ulanzi TC001](https://www.ulanzi.com/products/ulanzi-pixel-smart-clock-2882) smart clock running [AWTRIX 3 firmware](https://blueforcer.github.io/awtrix3/)
- MQTT broker ([Mosquitto](https://www.home-assistant.io/integrations/mqtt/) recommended)

## Usage

Each blueprint directory contains:
- Installation instructions
- Configuration options
- Required integrations

## License

MIT License - see [LICENSE](LICENSE)
