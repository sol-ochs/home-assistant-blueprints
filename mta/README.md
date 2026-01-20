# MTA Subway Times to Ulanzi/AWTRIX Display

Display the next 3 subway arrival times on your Ulanzi/AWTRIX clock.

## Features

- Shows next 3 train arrival times in minutes
- Updates automatically when sensor values change
- Configurable MQTT device and app name

## Requirements

### Home Assistant

- Home Assistant
- MQTT broker (e.g., Mosquitto)
- [GTFS Realtime](https://www.home-assistant.io/integrations/gtfs_rt/) integration configured with MTA feeds

### Ulanzi/AWTRIX

- Ulanzi TC001 running AWTRIX 3 firmware
- Subway line icon downloaded to device (e.g., 72094 for Q train)

## Finding Your Subway Line Icon

1. Go to [LaMetric Icon Gallery](https://developer.lametric.com/icons)
2. Search for your subway line (e.g., "Q train", "A train", "1 train")
3. Create your own if it does not exist
3. Copy the icon ID number
4. Download the icon to your AWTRIX device via its web interface
5. Enter the icon ID when configuring the blueprint