<h1 align="center">🚀 ESP32 OTA Firmware Update System</h1> <p align="center"> <img src="https://img.shields.io/badge/Platform-ESP32-blue?style=for-the-badge"> <img src="https://img.shields.io/badge/Firmware-Auto_Update-green?style=for-the-badge"> <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge"> <img src="https://img.shields.io/github/license/MohdMusharrafGit/esp32-ota-firmware?style=for-the-badge"> </p>
🧩 Project Overview

This project enables secure HTTPS Over-The-Air (OTA) firmware updates for the ESP32 microcontroller.
Your ESP32 automatically checks a GitHub-hosted repository every few minutes for a newer firmware version, downloads it securely, and flashes itself — no manual intervention required!

✨ Key Highlights

🔒 HTTPS-based firmware delivery from GitHub

🔁 Auto-check for updates every 30 minutes

⚡ Seamless firmware download and self-flashing

🧠 Version control via version.txt

🧰 Lightweight, library-optimized design

⚙️ How It Works

ESP32 boots and connects to Wi-Fi.

It fetches version.txt from the GitHub repo.

Compares it to its internal firmware version.

If a newer version exists → it automatically downloads firmware.bin and installs it.

ESP32 reboots and runs the latest firmware.

📁 Repository Structure
📦 esp32-ota-firmware/
 ┣ 📜 firmware.bin       # Compiled binary firmware file
 ┣ 📜 version.txt        # Contains version number (e.g., 1.1.0)
 ┣ 📜 README.md          # You are here!

🧰 How to Upload New Firmware

Compile your new firmware (.bin)
In Arduino IDE → Sketch > Export Compiled Binary

Update version.txt

1.2.0


Upload both files to GitHub

Go to your repo → Click “Add file” → “Upload files”

Upload new firmware.bin and updated version.txt

Commit changes

ESP32 detects and updates automatically
Within 30 minutes (or your set interval), ESP32 will:

Detect new version

Download firmware securely

Flash and reboot 🎉

🧠 Example Serial Monitor Output
✅ WiFi connected!
🔍 Checking for new firmware...
Current Version: 1.0.0
Available Version: 1.1.0
🆕 New firmware found! Starting OTA update...
⬇️ Downloading... 100%
🎉 Update complete. Rebooting...

🧪 Tested On

ESP32 DevKit v1

Arduino IDE 2.x

Firmware up to 1MB OTA

🧑‍💻 Author

Mohd Musharraf
🎓 Central University of Jammu | ECE (Avionics)
💼 Interested in Embedded Systems, IoT & Avionics
🔗 GitHub Profile

📜 License

This project is licensed under the MIT License
.

<p align="center">⭐ Star this repo if you found it helpful!</p>
