# Dexcom to AWTRIX Display

Display real-time Dexcom glucose readings with trend arrows on your Ulanzi smart clock.

<img src="screenshot.png" alt="Screenshot" width="400">

## Requirements

- [Dexcom integration](https://www.home-assistant.io/integrations/dexcom/) with sensors:
  - `sensor.{username}_glucose_value` - Glucose reading (mg/dL)
  - `sensor.{username}_glucose_trend` - Trend direction
- Icon ID `8192` on AWTRIX device (customizable)

## Installation

1. Download icon `8192` to your AWTRIX device (or use a different icon ID). Instructions here: [AWTRIX 3 - Icons](https://blueforcer.github.io/awtrix3/#/icons?id=icons)
2. Import blueprint: Settings → Automations & Scenes → Blueprints → Import Blueprint
3. Paste URL: `https://raw.githubusercontent.com/sol-ochs/home-assistant-blueprints/main/dexcom/blueprint.yml`
4. Create automation and configure:
   - Glucose value sensor (e.g., `sensor.username_glucose_value`)
   - Glucose trend sensor (e.g., `sensor.username_glucose_trend`)
   - MQTT topic (default: `awtrix/custom/dexcom`)

## Troubleshooting

- **"???" displays:** Sensor data unavailable or invalid
- **No updates:** Check MQTT broker connection and topic configuration
- **Wrong arrow or "?":** Verify trend sensor values match expected states
