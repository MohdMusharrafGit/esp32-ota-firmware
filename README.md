<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ESP32 HTTPS OTA Updater</title>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: "Poppins", sans-serif;
      background: linear-gradient(120deg, #0f2027, #203a43, #2c5364);
      color: #fff;
      padding: 40px;
    }
    header {
      text-align: center;
      margin-bottom: 50px;
    }
    header h1 {
      font-size: 2.8rem;
      color: #00c8ff;
      letter-spacing: 2px;
    }
    header p {
      color: #b5c8d1;
      font-size: 1.2rem;
    }
    .card {
      background: rgba(255, 255, 255, 0.1);
      border-radius: 20px;
      padding: 30px;
      margin-bottom: 30px;
      backdrop-filter: blur(10px);
      box-shadow: 0 4px 20px rgba(0,0,0,0.3);
    }
    h2 {
      color: #00c8ff;
      border-left: 4px solid #00c8ff;
      padding-left: 10px;
      margin-bottom: 15px;
    }
    ul, ol {
      margin-left: 20px;
    }
    pre {
      background: #1b2a38;
      padding: 15px;
      border-radius: 10px;
      overflow-x: auto;
      color: #00ffb3;
    }
    footer {
      text-align: center;
      margin-top: 40px;
      color: #aaa;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>

  <header>
    <h1>🚀 ESP32 HTTPS OTA Updater</h1>
    <p>Secure Over-The-Air Firmware Updates | Powered by GitHub + HTTPS</p>
  </header>

  <div class="card">
    <h2>🌟 Project Overview</h2>
    <p>
      This ESP32 project enables seamless Over-The-Air (OTA) firmware updates using secure HTTPS communication.  
      The device periodically checks a hosted GitHub repository for new firmware releases and updates automatically — no manual flashing needed.
    </p>
  </div>

  <div class="card">
    <h2>⚙️ Core Features</h2>
    <ul>
      <li>Automatic firmware version checking every 30 minutes</li>
      <li>Secure HTTPS communication with GitHub</li>
      <li>Fail-safe OTA update process with progress tracking</li>
      <li>Reboots automatically after successful flash</li>
      <li>Fully open-source implementation</li>
    </ul>
  </div>

  <div class="card">
    <h2>🧱 File Structure</h2>
    <pre>
📦 esp32-ota-firmware
 ┣ 📜 firmware.bin
 ┣ 📜 version.txt
 ┗ 📜 README.html
    </pre>
  </div>

  <div class="card">
    <h2>🧪 Example Output</h2>
    <pre>
✅ WiFi connected!
IP address: 192.168.1.25
🔍 Checking for new firmware...
Current Version: 1.0.0
Available Version: 1.1.0
🆕 New firmware found! Starting OTA update...
⬇️ Downloading... 100%
🎉 Update complete. Rebooting...
    </pre>
  </div>

  <div class="card">
    <h2>👨‍💻 Author</h2>
    <p>
      Developed by <strong>Mohd Musharraf</strong>  
      under guidance from <em>Advancetech Pvt. Ltd.</em>  
      Project Type: Research + Development | Field: IoT & Embedded Systems
    </p>
  </div>

  <footer>
    <p>© 2025 ESP32 OTA Project | Built with ❤️ by Mohd Musharraf</p>
  </footer>

</body>
</html>
