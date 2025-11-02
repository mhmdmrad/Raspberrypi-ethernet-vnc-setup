

## Table of Contents
1. [Requirements](#requirements)
2. [Download and Flash Raspberry Pi OS](#download-and-flash-raspberry-pi-os)
3. [Enable SSH and Configure Wi-Fi (Optional)](#enable-ssh-and-configure-wi-fi-optional)
4. [Connect Raspberry Pi via Ethernet to Router](#connect-raspberry-pi-via-ethernet-to-router)
5. [Find Raspberry Pi IP Address](#find-raspberry-pi-ip-address)
6. [Connect to Raspberry Pi using SSH](#connect-to-raspberry-pi-using-ssh)
7. [Enable VNC on Raspberry Pi](#enable-vnc-on-raspberry-pi)
8. [Connect via RealVNC Viewer](#connect-via-realvnc-viewer)
9. [Troubleshooting](#troubleshooting)
10. [Credits](#credits)

---

## Requirements


- Raspberry Pi 4 Model B (8GB recommended)
- microSD card (minimum 16GB)
- Raspberry Pi Imager v1.7.3 or newer
- Ethernet cable
- Wi-Fi router with internet access
- Laptop or PC on the same network
- Angry IP Scanner
- RealVNC Viewer

---

# Download and Flash Raspberry Pi OS

1. Go to: https://www.raspberrypi.com/software/
2. Download Raspberry Pi Imager (for Windows).
3. Insert your microSD card into your computer.
4. Open Raspberry Pi Imager.
5. Choose OS:
   - Raspberry Pi OS (64-bit) → Full version.
6. Choose Storage:
   - Select your microSD card.
7. Click the gear icon (⚙️) for advanced settings:
   - Set hostname: raspberrypi
   - Enable SSH
   - Username: pi
   - Password: raspberry
   - Set Wi-Fi (optional, if needed later)
   - Set locale (timezone and keyboard)
8. Click **Save**, then **Write**.
9. When finished, eject the SD card safely.

---

# Enable SSH and Configure Wi-Fi manually
## If SSH or Wi-Fi were not configured in Imager:

1. Reinsert the SD card into your computer.
2. In the root directory, create an empty file named: ssh
3. Create another file named: wpa_supplicant.conf
4. Open wpa_supplicant.conf and paste the following:

```
country=LB  //Put your own country /GB/US/ etc..
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1

network={
    ssid="YOUR_WIFI_NAME"
    psk="YOUR_WIFI_PASSWORD"
}
   ```
5. Save the file and safely eject the SD card again.

---

# Connect Raspberry Pi via Ethernet to Router
1. Insert the SD card into your Raspberry Pi.
2. Connect one end of the Ethernet cable to the Raspberry Pi.
3. Connect the other end to your router’s LAN port.
4. Power on the Raspberry Pi using its USB-C power adapter.
5. Wait about 1–2 minutes for the Pi to boot completely.

---
# Find Raspberry Pi IP Address

1. Download Angry IP Scanner: https://angryip.org/download/
2. Open Angry IP Scanner and scan your local network range (example: 192.168.1.0 – 192.168.1.255).
3. Look for a device named "raspberrypi".
4. Note its IP address, for example: 192.168.1.11










































