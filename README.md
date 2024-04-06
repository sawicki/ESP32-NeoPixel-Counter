# ESP32 LED Controller

## Overview
This project uses an ESP32 to quickly find the number of Pixels in your WS2812 type string.

## Features
- WiFi connectivity for straightforward setup and control.
- Web interface with intuitive sliders for LED control.
- Support for up to 1000 WS2812 LEDs.
- Customizable settings for both LEDs and WiFi.

## Prerequisites
- An ESP32 microcontroller.
- A WS2812 LED strip.
- A basic understanding of electronics and Arduino IDE programming.

## Installation
### Hardware Setup
1. Connect the data input of your WS2812 LED strip to the appropriate pin on the ESP32.
2. Ensure the LED strip is powered correctly, adhering to its specification.

### Software Setup
1. Download and install the Arduino IDE on your computer.
2. Add the ESP32 board to your Arduino IDE:
   - Instructions can be found [here](https://github.com/espressif/arduino-esp32/blob/master/docs/arduino-ide/boards_manager.md).
3. Install the necessary libraries via the Arduino Library Manager:
   - `WiFi`
   - `WebServer`
   - `Adafruit NeoPixel`
   - `WiFiManager`
4. Clone this repository or download the project code.
5. Open the project in Arduino IDE.
6. Select your ESP32 board from the `Tools > Board` menu.
7. Upload the code to your ESP32.

## Usage
1. Once powered on, the ESP32 will automatically create a WiFi access point named `ESP32_AP`.
2. Connect to this WiFi network with any WiFi-enabled device.
3. A captive portal should automatically appear to configure your WiFi connection. If not, go to `http://192.168.4.1`.
4. After connecting to your home WiFi, the ESP32 will display its IP address in the Serial Monitor.
5. Open a web browser and navigate to the provided IP address.
6. Use the sliders on the web interface to adjust the LEDs on your strip.


## License
This project is released under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- A big thank you to the developers of the Adafruit NeoPixel and WiFiManager libraries for enabling this project. This sketch and the readme was largely written by ChatGPT 4.
