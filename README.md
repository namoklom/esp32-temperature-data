# ESP32 Sensor Data Gathering API Using Flask

## 👤 Author

| Name            | Role              | LinkedIn                                      |
|-----------------|-------------------|-----------------------------------------------|
| Jason Emmanuel  | Back-End Developer | [linkedin.com/in/jasoneml](https://www.linkedin.com/in/jasoneml/) |

This project provides a simple RESTful API built with Flask, designed to receive environmental sensor data—specifically temperature and humidity—sent from an ESP32 microcontroller device. The API accepts HTTP POST requests with JSON payloads, validates and processes the data, and responds with confirmation or error messages.

This project serves as a backend server for IoT applications where ESP32 or similar microcontroller devices send sensor data to be collected, stored, or further processed.

---

## Overview

This project demonstrates how to build a lightweight Flask web server that can receive data from an ESP32 device over the network. The ESP32 collects temperature and humidity values from sensors (like DHT11/DHT22) and sends this data as JSON to the Flask API endpoint.

The Flask server:

- Accepts JSON POST requests at `/data`.
- Checks that the incoming data contains the required fields (`temperature` and `humidity`).
- Returns a JSON response confirming success or reporting errors.
- Prints received data to the console for monitoring.

This backend could be further extended to store data in a database, trigger alerts, or visualize sensor readings.

---

## Features

- Simple and easy-to-understand Flask REST API
- Receives sensor data (temperature & humidity) from IoT devices
- Validates JSON data and handles missing or invalid input gracefully
- Returns clear JSON success or error responses
- Prints incoming data for server-side monitoring
- Lightweight and suitable for small-scale IoT projects

---

## Setup Instructions

### Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.x: https://www.python.org/downloads/
- pip (Python package installer)
- Flask library: Install via pip
- An ESP32 development board with Wi-Fi connectivity

## Tools and Libraries

| Tool / Library        | Purpose                                           | Installation / Reference                         |
|----------------------|-------------------------------------------------|-------------------------------------------------|
| Python 3.x           | Programming language for the Flask server       | https://www.python.org/downloads/                |
| Flask                | Web framework to build the REST API              | `pip install flask`                              |
| ESP32                | Microcontroller to collect and send sensor data | https://www.espressif.com/en/products/hardware/esp32/overview |
| Arduino IDE / PlatformIO | Development environment for ESP32               | https://www.arduino.cc/en/software               |
| HTTPClient (Arduino) | Library to send HTTP requests from ESP32         | Included in Arduino ESP32 core                    |
| WiFi Library (Arduino)| To connect ESP32 to Wi-Fi network                 | Included in Arduino ESP32 core                    |
| curl                 | Command-line tool to test API                      | Usually pre-installed on Linux/macOS, Windows via https://curl.se/ |
| Postman              | GUI tool for API testing and development          | https://www.postman.com/downloads/                |
