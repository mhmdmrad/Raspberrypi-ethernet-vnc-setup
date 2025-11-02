
# Table of Contents
1. [Requirements](#requirements)
2. [Download and Flash Raspberry Pi OS](#download-and-flash-raspberry-pi-os)
3. [Enable SSH and Configure Wi-Fi (Optional)](#enable-ssh-and-configure-wi-fi-optional)
4. [Connect Raspberry Pi via Ethernet](#connect-raspberry-pi-via-ethernet)
5. [Find Raspberry Pi IP Address](#find-raspberry-pi-ip-address)
6. [Connect to Raspberry Pi using SSH](#connect-to-raspberry-pi-using-ssh)
7. [Enable VNC on Raspberry Pi](#enable-vnc-on-raspberry-pi)
8. [Connect via RealVNC Viewer](#connect-via-realvnc-viewer)
9. [Troubleshooting](#troubleshooting)
10. [Credits](#credits)

---

# Requirements

```bash
- Raspberry Pi 4 Model B (8GB recommended)
- microSD card (at least 16GB)
- Raspberry Pi Imager (v1.7.3 or later)
- Ethernet cable
- Laptop or PC running Windows 10 or newer
- RealVNC Viewer
- Angry IP Scanner
```
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

# Enable SSH and Configure Wi-Fi (Optional)
## If you skipped enabling SSH or Wi-Fi or if your  in Raspberry Pi Imager :
