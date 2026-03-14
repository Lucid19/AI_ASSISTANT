# AI ASSISTANT 🚀
Designed as an ESP32 based board for TTS (Text to Speech) and STT (Speech to Text) communicating with AI API through enabled WiFi. Set up with an Electret Condenser Microphone and 1W speaker with an amplified signal. This board is suitable for hobbyists and is capable of being hand soldered.

## 📋 Features
* ⚡ Input Voltage: 3.3V - 10V
* 🧩 MCU: ESP32-S3-WROOM (WiFi enabled)
* 📢 Speaker: 1W 8ohm impedance (SP-4005Y)
* 📏 Size: 95x65mm
* 🔌 USB-C charging and programming

## 🔌 Pinout
* | RX | UART | Do not connect during firmware update |
* | TX | UART |
* | GPIO35 | SPI/GENERIC | I/O
* | GPIO36 | SPI/GENERIC | I/O
* | GPIO37 | SPI/GENERIC | I/O
* | GPIO38 | GENERIC/RGB | I/O
* | GPIO39 | JTAG (MTCK) | I/O
* | GPIO40 | JTAG (MTDO) | I/O 
* | GPIO41 | JTAG (MTDI) | I/O
* | GPIO42 | JTAG (MTMS) | I/O

(RTC Supported)
* | GPIO13 | Digital I/O, PWM, SPI/I2C/UART | I/O
* | GPIO14 | Digital I/O, PWM, SPI/I2C/UART | I/O
* | GPIO15 | Digital I/O, PWM, SPI/I2C/UART | I/O
* | GPIO16 | Digital I/O, PWM, SPI/I2C/UART | I/O
* | GPIO21 | Digital I/O, PWM, SPI/I2C/UART | I/O
  
* | A2-A9 | Analog sensing interface | Input |

Note: This board is NOT compatible with Octal PSRAM (R8) modules. Use Quad SPI (N4/N8/R2) versions only.

## 🛠 Setup & Usage
Programmable using Arduino IDE or VS Code + PlatformIO
To upload code:
1. Short the Boot Jumper
2. Press and release the Reset button (or toggle the power). The chip "looks" at GPIO 0, sees it is Low, and enters Download Mode.
3. Start the upload in your software (Arduino/PlatformIO).
4. Once finished, remove the jumper.
5. Press Reset again to run your code.

## 📦 Key Components
* ESP32-S3-WROOM
* TPC114S1-VR LDO Regulator
* PAM8406DR Sound Amplifier
* CMA-4544PF-W Electret Condenser Microphone
* USB-C 16-pin Connector

## estimated price (as of 14/03/26)
£13.60 (components) + £3.76-£6.78 (JLPCB)
= £17.36-£20.38 + shipping fees

---
*Created by Daumantas Dauksas - 2026*
