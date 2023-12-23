# mqtt_config_control
Requirements
•	Hardware:
  •	ESP8266 board (e.g., NodeMCU)
  •	Relays and corresponding devices (e.g., light bulbs) connected to the GPIO pins of the ESP8266.
  •	Software:
  •	Arduino IDE - The development environment for programming the ESP8266.
  •	Libraries:
  •	ESP8266WiFi - WiFi connectivity for ESP8266.
  •	PubSubClient - MQTT client library for ESP8266.
  •	ArduinoJson - Library for handling JSON data in Arduino projects.
  
Setup Instructions
  1.	Install Arduino IDE:
    •	Download and install the Arduino IDE from the official website.
  2.	Install Required Libraries:
    •	Open Arduino IDE.
    •	Go to Sketch -> Include Library -> Manage Libraries.
    •	Search for the following libraries and install them:
    •	ESP8266WiFi by ESP8266 Community
    •	PubSubClient by Nick O'Leary
    •	ArduinoJson by Benoit Blanchon
  3.	Hardware Setup:
    •	Connect your ESP8266 board to the relays and respective devices (e.g., light bulbs) according to your circuit design.
  4.	Code Upload:
    •	Open the provided Arduino sketch in this repository in Arduino IDE.
    •	Update the WiFi SSID, password, MQTT broker details, and other configuration settings in the code.
    •	Upload the code to your ESP8266 board.
  5.	Serial Monitor (Optional):
    •	Open the serial monitor in Arduino IDE (Tools -> Serial Monitor) to view debug information and MQTT messages.
  6.	Test MQTT Communication:
    •	Use an MQTT client (e.g., MQTT Explorer) to publish messages to the configured topics (mqtt/config and mqtt/control) to control the relays.

Usage
  •	After uploading the code and establishing the connections, the ESP8266 will connect to the configured WiFi network and MQTT broker.
  •	Publish configuration JSON messages to mqtt/config to define relay counts and states.
  •	Publish control JSON messages to mqtt/control to control the relays based on the specified relay number and state.

Contributing
  • Feel free to contribute by opening issues or pull requests, reporting bugs, or suggesting improvements.

License
  • This project is licensed under the [License Name] License - see the LICENSE.md file for details.

