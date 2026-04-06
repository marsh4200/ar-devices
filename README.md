# ar-devices


🔧 # AR Smart Home – ESPHome Devices

This repository contains ready-to-use ESPHome configurations and packages for AR Smart Home devices.

It includes support for:

M5 Series (1G / 2G / 3G)
TX Series (1G / 2G / 3G)
🚀 Getting Started

Follow these steps to flash and use your device.

📥 1. Download a Template

Go to the templates folder and download the correct config:

m5-1g-config.yaml
m5-2g-config.yaml
m5-3g-config.yaml
tx-1g-config.yaml
tx-2g-config.yaml
tx-3g-config.yaml
✏️ 2. Edit the Config

Open the file and update the required fields:

substitutions:
  device_name: "YOUR_DEVICE_NAME"
  friendly_name: "YOUR_FRIENDLY_NAME"

wifi:
  ssid: "YOUR_WIFI_NAME"
  password: "YOUR_WIFI_PASSWORD"

api:
  encryption:
    key: "YOUR_API_KEY"

ota:
  password: "YOUR_OTA_PASSWORD"
➕ 3. Add to ESPHome
Open ESPHome
Click New Device
Choose Continue without installing
Paste your edited YAML file
Save
⚡ 4. Flash the Device
Click Install
Select Manual Download
Download the .bin file
Flash the device via USB
🔌 5. Power Up
Install the device physically
Power it on
🏠 6. Home Assistant
The device will appear automatically in Home Assistant
Entities will be created based on the device type:
Device	Entities
1G	1 switch
2G	2 switches
3G	3 switches
📦 How It Works
Templates = user configuration (WiFi, name, etc.)
Packages = device logic (pins, relays, buttons)

This allows:

Easy setup for users
Central updates from GitHub
Consistent device behavior
⚠️ Notes
Updating packages on GitHub does not automatically update devices
Devices must be re-installed or updated via OTA
GPIO9/GPIO10 on TX devices may vary depending on hardware
✅ Done

Your device is now ready and fully integrated with Home Assistant.

🔥 AR Smart Home

Built for simple, scalable, and professional smart home installations.
