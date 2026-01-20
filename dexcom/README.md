# Dexcom to AWTRIX Display

Display real-time Dexcom glucose readings and trends on your Ulanzi/AWTRIX clock:

<img src="screenshot.png" alt="Screenshot" width="400">

## Features

- Real-time glucose values with trend arrows
- Custom arrow drawing commands  
  (AWTRIX does not support secondary icons or rendering ASCII arrow characters in text)
- Updates automatically when sensor values change

## Requirements

### Home Assistant

- Home Assistant
- MQTT broker (e.g., Mosquitto)
- [Dexcom integration](https://www.home-assistant.io/integrations/dexcom/) configured with account access

### Ulanzi/AWTRIX

- Ulanzi TC001 running AWTRIX 3 firmware
- Blood drop icon (ID: 8192) downloaded to device

## Troubleshooting

| Trouble | Shooting |
| - | - |
| "???" instead of reading | Sensor data unavailable or invalid |
| No updates | Check MQTT broker connection and topic configuration |
| "?" instead of trend arrow | Verify trend sensor values match expected states |
