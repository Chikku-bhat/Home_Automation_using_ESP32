# ESP32 (or ESP8266) Home Automation Server with Relay Control

This project enables you to turn your ESP32 (or ESP8266) microcontroller into a simple home automation server that allows you to control electrical devices remotely using relays. The server creates a web-based interface where you can toggle the state of connected devices through a web browser.

## Features

- Control up to 4 electrical devices using a 4-channel relay module.
- Create a Wi-Fi Access Point (AP) on the ESP32 (or ESP8266) for connecting and controlling devices.
- Web-based interface with buttons to turn relays on and off.
- Dynamically generated HTML pages that reflect the current state of the relays.
- Easy-to-understand codebase with comments for quick customization.

## Getting Started

1. Load the provided code onto your ESP32 (or ESP8266) microcontroller using your preferred development environment (Arduino IDE, PlatformIO, etc.).

2. Replace network credentials with your desired SSID and password in the code to create the Wi-Fi Access Point (AP).

3. Configure the GPIO pins to match the connections with the relay module. By default, GPIO pins 12, 14, and 27 are used to control relays.

4. Upload the code to your ESP32 (or ESP8266) and open the Serial Monitor to monitor the server's IP address.

5. Connect your computer or mobile device to the Wi-Fi network created by the ESP32 (or ESP8266).

6. Open a web browser and navigate to the IP address shown in the Serial Monitor to access the control interface.

## Usage

- The web interface will display the current state of each relay (on or off) along with buttons to control them.
- Click the "ON" button to turn a relay on and the "OFF" button to turn it off.
- The buttons' appearance will change dynamically based on the current state of each relay.

## Considerations

- This project provides a basic example of remote device control using relays. For production environments, consider adding security measures like authentication and HTTPS.
- You can easily customize the code to add more relays or devices, and improve error handling as needed.

## Dependencies

- WiFi library (included in Arduino IDE) for Wi-Fi connectivity.
- HTML and CSS for the web-based control interface.

## Compatibility

- The project is designed for ESP32 microcontrollers. For ESP8266, you'll need to replace `<WiFi.h>` with `<ESP8266WiFi.h>` and adjust the GPIO pins as needed.
