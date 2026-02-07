

# Life Pulse – Smart Heart Rate Monitoring System

Life Pulse is a smart heart rate monitoring system designed using an ESP32 and a Nokia 5110 LCD.  
The system measures heart rate in real time, displays clear medical-style information on the screen, and provides audio, visual, and remote alerts when abnormal heart rate values are detected.

This project simulates the behavior of real medical monitoring devices and is suitable for educational, research, and demonstration purposes.

---

## 📌 Features

- Real-time heart rate (BPM) monitoring
- Clean medical-style LCD interface (no waveform clutter)
- Title-based UI: **Life Pulse**
- Centered heart rate display
- Clear sensor status indication:
  - **OK**
  - **ALERT**
  - **NO SIGNAL**
- Audio alarm with medical-style pattern when HR > 100 BPM
- Visual alerts using LEDs
- Telegram notification for critical heart rate alerts
- Non-blocking system logic (millis-based timing)

---

## 🧠 System Behavior

| Condition | LCD Status | LED | Buzzer |
|---------|-----------|-----|--------|
| Normal HR (<100 BPM) | OK | Green | Short beep on beat |
| High HR (≥100 BPM) | ALERT | Red | High beep – pause – high beep |
| No sensor signal | NO SIGNAL | Off | Silent |

---

## 🛠 Hardware Components

- ESP32 Development Board  
- Heart Rate Sensor (Analog Output)  
- Nokia 5110 LCD (PCD8544)  
- Active Buzzer  
- Red LED  
- Green LED  
- Connecting wires  
- Power supply (USB / Battery)

---

## 📟 LCD Display Layout

Life Pulse

78 BPM
STATUS: OK

Example alert state:

Life Pulse

132 BPM
STATUS: ALERT

---

## 🌐 Connectivity

- WiFi-enabled (ESP32)
- Sends alerts via **Telegram Bot API**
- Secure HTTPS communication

---

## 📂 Project Structure

LifePulse/
│
├── LifePulse.ino        # Main Arduino code
├── README.md            # Project documentation

---

## 🚀 Getting Started

1. Clone this repository
2. Open the `.ino` file using Arduino IDE
3. Install required libraries:
   - Adafruit_GFX
   - Adafruit_PCD8544
4. Update WiFi credentials and Telegram Bot details
5. Upload the code to ESP32
6. Connect hardware components
7. Power on and monitor heart rate

---

## 🔒 Disclaimer

This project is intended for **educational and research purposes only**.  
It is **not a certified medical device** and should not be used for clinical diagnosis or treatment.

---

## 📜 License

This project is open-source and available under the **MIT License**.  
You are free to use, modify, and distribute it with proper attribution.

---

## 👤 Author

Developed by **Life Pulse Team**  
ESP32 • Embedded Systems • IoT • Health Monitoring

---

## ⭐ Acknowledgment

Inspired by real hospital ECG and heart monitoring devices to provide a realistic learning experience for students and researchers.

