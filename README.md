# ESP32-NeoPixel-Counter
ESP32 LED Controller
Overview
This project turns your ESP32 into a web-controlled LED strip controller, specifically designed for WS2812 LEDs. It leverages the ESP32's WiFi capabilities to host a web server, allowing users to control the color and brightness of individual LEDs or patterns on the strip via a simple web interface.

Features
WiFi connectivity for easy setup and control.
Web interface with sliders for intuitive LED control.
Supports up to 1000 WS2812 LEDs.
Customizable LED and WiFi settings.
Prerequisites
ESP32 microcontroller.
WS2812 LED strip.
Basic understanding of electronics and programming with Arduino IDE.
Installation
Hardware Setup
Connect your WS2812 LED strip's data input to GPIO 10 on the ESP32.
Ensure the LED strip is powered correctly, following its specifications.
Software Setup
Install the Arduino IDE on your computer.
Add the ESP32 board to the Arduino IDE:
Follow the instructions here.
Install the following libraries through the Arduino Library Manager:
WiFi
WebServer
Adafruit NeoPixel
WiFiManager
Clone this repository or download the code.
Open the project in the Arduino IDE.
Select your ESP32 board from the Tools > Board menu.
Upload the code to your ESP32.
Usage
Power on your ESP32. It will automatically create a WiFi access point named ESP32_AP.
Connect to this WiFi network with any WiFi-enabled device.
A captive portal should appear for configuring your WiFi connection. If not, navigate to http://192.168.4.1.
Once connected to your home WiFi, the ESP32 will print its IP address to the Serial Monitor.
Open a web browser and navigate to the IP address displayed.
Use the web interface sliders to control the LEDs on your strip.
Contributing
Contributions to the ESP32 LED Controller project are welcome! Here's how you can contribute:

Fork the repository.
Create a new branch for your feature or fix.
Commit your changes.
Push to your branch.
Submit a pull request.
License
This project is licensed under the MIT License - see the LICENSE file for details.
