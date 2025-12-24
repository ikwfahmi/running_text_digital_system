# 📟 Running Text Digital System (ESP32 + P10 LED Matrix)

A smart digital information board system powered by **ESP32** and **P10 LED Matrix**. This project allows users to display scrolling text, real-time data, or announcements with high visibility.

## 🚀 Overview

The **Running Text Digital System** is designed to replace traditional static signage with a dynamic, programmable LED display. By utilizing the processing power of the ESP32, this system can be expanded to include WiFi-based controls, NTP time synchronization, or remote updates via a web interface or mobile app.

## ✨ Key Features

* **Dynamic Scrolling:** Smooth scrolling text animation with adjustable speed.
* **High Visibility:** Uses P10 LED Matrix modules, suitable for both indoor and outdoor information boards.
* **ESP32 Powered:** High-performance processing and built-in WiFi/Bluetooth capabilities for future IoT expansion.
* **Customizable Content:** Easily update the text, font style, and brightness through the source code.
* **Modular Design:** Supports daisy-chaining multiple P10 modules for longer displays.

## 🛠️ Hardware Requirements

* **Microcontroller:** ESP32 (e.g., NodeMCU or DOIT DevKit V1)
* **Display:** P10 Single Color (usually Red) LED Matrix Module
* **Driver:** DMD (Dot Matrix Display) Connector or Jumper Wires
* **Power Supply:** 5V 2A (or higher depending on the number of P10 modules)
* **Level Shifter:** (Optional) To convert ESP32 3.3V logic to 5V for cleaner P10 signals.

## 🔌 Pin Mapping (Standard P10 to ESP32)

| P10 Pin | ESP32 GPIO | Function |
| :--- | :--- | :--- |
| **OE** | GPIO 21 | Output Enable |
| **A** | GPIO 19 | Address A |
| **B** | GPIO 18 | Address B |
| **CLK** | GPIO 14 | Clock |
| **SCLK** | GPIO 04 | Latch / SCLK |
| **DATA** | GPIO 23 | MOSI / Data |
| **GND** | GND | Ground |

## 📦 Required Libraries

To compile this project, ensure you have the following libraries installed in your Arduino IDE:

1.  `DMD32` (Specifically optimized for ESP32)
2.  `Adafruit GFX Library`
3.  `TimerOne` (or equivalent interrupt timer for ESP32)

## ⚙️ Installation

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/ikwfahmi/running_text_digital_system.git](https://github.com/ikwfahmi/running_text_digital_system.git)
    ```
2.  **Open Project:** Open the `.ino` file located in the project folder using Arduino IDE.
3.  **Library Setup:** Install the required libraries mentioned above.
4.  **Board Selection:** Select **DOIT ESP32 DEVKIT V1** (or your specific ESP32 model) in `Tools > Board`.
5.  **Upload:** Connect your ESP32 and click the **Upload** button.

## 🖥️ Usage

Once uploaded, the system will initialize the DMD buffer and begin scrolling the pre-programmed text. 

> **Note:** If the display appears scrambled, check your wiring pins and ensure the 5V power supply is sufficient, as the ESP32 USB power is often not enough to drive the full LED matrix.

## 🤝 Contributing

Contributions are welcome! If you have ideas for WiFi-based control interfaces or new animation styles, feel free to:
1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.

---
*Developed by [ikwfahmi](https://github.com/ikwfahmi)*
