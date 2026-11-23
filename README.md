# fardriver-display-app
# ⚡ FarDriver Live BLE Dashboard

A clean, modern, real-time web telemetry dashboard for **FarDriver** motor controllers over **Bluetooth Low Energy (BLE)**. Built as a lightweight Progressive Web App (PWA) optimized for mobile screens during rides.

🔗 **Live App:** [https://noam1534.github.io/fardriver-display-app/](https://noam1534.github.io/fardriver-display-app/)

---

## ✨ Features

* **Real-Time Telemetry:** Displays live Speed (KM/H), RPM, Battery Voltage (V), Estimated Battery Percentage, Instantaneous Power (W), Battery Line Current (A), Phase Current (A), Controller/Motor Temperatures, and Active Gear.
* **Direct BLE Connection:** Connects straight to standard FarDriver BLE dongles (`0xFFE0` / `0xFFE1` UART-over-BLE service) without extra hardware.
* **Custom Wheel & Motor Calibration:** Adjustable wheel diameter (inches) and motor pole pairs for accurate speed calculation.
* **Built-in Demo / Simulation Mode:** Test the UI and gauges anytime without being connected to the controller.
* **Raw Hex Stream Monitor:** Live packet inspector at the bottom of the screen to verify and fine-tune firmware byte offsets.

---

## 📱 How to Run on iPhone (iOS)

Because standard mobile Safari does not support the **Web Bluetooth API**, follow these steps to run the dashboard on iOS:

1. Download **Bluefy – Web BLE Browser** (free on the App Store).
2. Open Bluefy and navigate to:  
   `https://noam1534.github.io/fardriver-display-app/`
3. Tap **התחבר לבקר (Connect)** and select your FarDriver Bluetooth dongle.

*(On Android or Desktop, you can open the link directly in **Google Chrome** or **Microsoft Edge**).*

---

## 🛠️ Tech Stack

* **Frontend:** Vanilla HTML5, CSS3 (Dark Mode UI), JavaScript (ES6+)
* **Connectivity:** Web Bluetooth API (`0xFFE0` Service / `0xFFE1` Characteristic)
* **Hosting:** GitHub Pages

---

## ⚠️ Disclaimer

This dashboard is for informational and telemetry display purposes only. Always ride safely and verify critical battery and temperature limits against your controller's official configuration.
