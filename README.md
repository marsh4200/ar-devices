# 🔧 AR Smart Home – ESPHome Devices

This repository contains ready-to-use ESPHome configurations and packages for AR Smart Home devices.

## Supported Devices
- M5 Series (1G / 2G / 3G)
- M5 Series With Double Click
- TX Series (1G / 2G / 3G)
- POWR320
- DualR3 Lite
- MiniR4-Extreme
- 4ch-Pro-R3
- MiniR2
- Basic-R2

---

## 🚀 Getting Started

Follow these steps to flash and use your device.

---

## 📥 1. Download a Template

Go to the **templates folder** and download the correct config:

- m5-1g-config.yaml  
- m5-2g-config.yaml  
- m5-3g-config.yaml
- m5-1g-advanced-config.yaml
- m5-2g-advanced-config.yaml
- m5-3g-advanced-config.yaml
- tx-1g-config.yaml  
- tx-2g-config.yaml  
- tx-3g-config.yaml
- powr320-config.yaml
- dualr3lite-config.yaml
- minir4-extreme-config.yaml
- 4ch-pro-r3-config.yaml
- minir2-config.yaml
- basic-r2-config.yaml

---

## ✏️ 2. Edit the Config

Open the file and update:

```
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
```

---

## ➕ 3. Add to ESPHome

- Open ESPHome  
- Click **New Device**  
- Select **Continue without installing**  
- Paste your edited YAML  
- Save  

---

## ⚡ 4. Flash the Device

- Click **Install**  
- Select **Manual Download**  
- Download the `.bin` file  
- Flash via USB  

---

## 🔌 5. Power Up

- Install the device physically  
- Power it on  

---

## 🏠 6. Home Assistant

- Device will appear automatically  
- Entities are created based on type:

| Device | Entities |
|--------|---------|
| 1G     | 1 switch |
| 2G     | 2 switches |
| 3G     | 3 switches |

---

## 📦 How It Works

- Templates = user configuration  
- Packages = device logic  

### Benefits:
- Easy setup  
- Central updates  
- Consistent behavior  

---

## ⚠️ Notes

- GitHub updates do NOT auto-update devices  
- Devices must be updated manually or via OTA  
- GPIO9/GPIO10 on TX devices may vary  

---

## ✅ Done

Your device is now ready and integrated with Home Assistant.

---

# 🔥 AR Smart Home (Pty) Ltd
Built for simple, scalable, and professional smart home installations.
