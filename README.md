# Interface 1.8-inch TFT Graphic Display with Raspberry Pi Pico (MicroPython)

A complete step-by-step guide and MicroPython script to interface a 1.8-inch TFT Graphic Display (ST7735 Driver) with a Raspberry Pi Pico using SPI communication.

---

## 🛠️ Required Components
* Raspberry Pi Pico (with headers)
* 1.8-inch TFT LCD Display Module (ST7735, 128x160 resolution)
* Breadboard (830 Point)
* Jumper Wires (Male-to-male, 7 pieces)
* Micro USB Data Cable

---

## ⚡ Circuit Connections (Pinout)

| Raspberry Pi Pico Pin | TFT LCD Display Pin | Function / Description |
| :--- | :--- | :--- |
| **GP18** | CS | Chip Select |
| **GP17** | RST | Reset |
| **GP16** | RS (DC) | Register Select / Data Command |
| **GP11** | SDA (MOSI) | Data Line |
| **GP10** | CLK (SCK) | Clock Line |
| **GND** | GND | Ground |
| **3V3 (OUT)** | 3.3V | Power Supply (Must be 3.3V) |

> ⚠️ **Important Warning:** Both the power supply and data pins operate strictly at **3.3V**. Applying 5V will permanently damage your display.

---

## 📚 Library Installation
This project requires two MicroPython libraries:
1. `ST7735.py`
2. `sysfont.py`

Upload both library files directly to your Raspberry Pi Pico using **Thonny IDE** (`File > Save As... > Raspberry Pi Pico`).

---

## 🚀 How to Run
1. Connect the circuit as shown in the pinout table.
2. Upload the required libraries (`ST7735.py`, `sysfont.py`) to the Pico.
3. Open and run the `tft-pico.html` or python script inside Thonny IDE.

---

## 📄 License
This project is open-source and available for hobbyists, students, and developers.