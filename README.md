<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ESP32 HTTPS OTA Updater</title>
  <style>
    body {
      font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
      margin: 40px;
      background: #f8f9fb;
      color: #222;
      line-height: 1.6;
    }
    h1, h2, h3 {
      color: #0077cc;
    }
    code {
      background: #eee;
      padding: 2px 6px;
      border-radius: 4px;
      font-size: 14px;
    }
    pre {
      background: #282c34;
      color: #f8f8f2;
      padding: 10px;
      border-radius: 6px;
      overflow-x: auto;
    }
    a {
      color: #0077cc;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    .section {
      margin-bottom: 30px;
    }
  </style>
</head>
<body>

  <h1>🚀 ESP32 HTTPS OTA Updater</h1>
  <p>
    This project implements <strong>Over-The-Air (OTA)</strong> firmware updates on the <strong>ESP32</strong> using a <strong>secure HTTPS server</strong>.
    It automatically checks for new firmware every 30 minutes and updates the device when a newer version is found on GitHub.
  </p>

  <div class="section">
    <h2>📦 Features</h2>
    <ul>
      <li>Automatic OTA firmware updates via HTTPS</li>
      <li>Version-controlled updates using <code>version.txt</code></li>
      <li>Secure download from GitHub-hosted binary</li>
      <li>Automatic periodic update checks</li>
      <li>Serial logs for debugging and status updates</li>
    </ul>
  </div>

  <div class="section">
    <h2>⚙️ How It Works</h2>
    <ol>
      <li>ESP32 connects to Wi-Fi and retrieves <code>version.txt</code> from your GitHub repository.</li>
      <li>If a new version is detected, the new <code>.bin</code> file is downloaded securely via HTTPS.</li>
      <li>ESP32 performs a flash update and automatically reboots into the new firmware.</li>
    </ol>
  </div>

  <div class="section">
    <h2>🧰 Requirements</h2>
    <ul>
      <li>ESP32 board</li>
      <li>Arduino IDE with ESP32 core installed</li>
      <li>WiFi connection</li>
      <li>GitHub repository containing <code>firmware.bin</code> and <code>version.txt</code></li>
    </ul>
  </div>

  <div class="section">
    <h2>📁 GitHub File Structure</h2>
    <pre>
📦 esp32-ota-firmware
 ┣ 📜 firmware.bin
 ┣ 📜 version.txt
 ┗ 📜 README.md
    </pre>
  </div>

  <div class="section">
    <h2>🚀 Example Output (Serial Monitor)</h2>
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

  <div class="section">
    <h2>🧠 Author</h2>
    <p>
      Developed by <strong>Mohd Musharraf</strong> at <em>Advancetech Pvt. Ltd.</em>  
      For educational and research purposes.  
    </p>
  </div>

  <div class="section">
    <h2>📄 License</h2>
    <p>This project is open-source under the MIT License.</p>
  </div>

</body>
</html>
