# ESP32 Microcontroller Data Gathering with Embedded C++

## 👤 Author

| Name            | Role              | LinkedIn                                      |
|-----------------|-------------------|-----------------------------------------------|
| Jason Emmanuel  | Back-End Developer | [linkedin.com/in/jasoneml](https://www.linkedin.com/in/jasoneml/) |

This project demonstrates a lightweight backend solution to collect environmental sensor data from an ESP32 microcontroller device. Using Flask, a simple RESTful API is created to receive temperature and humidity data sent over HTTP POST requests in JSON format.

The ESP32 device, equipped with sensors like DHT11 or DHT22, gathers real-time environmental data and sends it to the Flask API endpoint `/data`. The backend validates incoming data, responds with clear success or error messages, and prints the data on the server console for monitoring.

This project can serve as the foundation for IoT applications including home automation, environmental monitoring, and data logging systems.

---

## 🚀 Overview

This project demonstrates how to build a lightweight Flask web server that can receive data from an ESP32 device over the network. The ESP32 collects temperature and humidity values from sensors (like DHT11/DHT22) and sends this data as JSON to the Flask API endpoint.

The Flask server:

- Accepts JSON POST requests at `/data`.
- Checks that the incoming data contains the required fields (`temperature` and `humidity`).
- Returns a JSON response confirming success or reporting errors.
- Prints received data to the console for monitoring.

This backend could be further extended to store data in a database, trigger alerts, or visualize sensor readings.

---

## ✨ Features

- RESTful API using Flask for simple data reception
- Supports JSON POST requests with temperature and humidity data
- Data validation to ensure completeness and correctness
- Meaningful JSON responses for success and errors
- Console logging for real-time data monitoring
- Easy to extend with database storage or notification systems
- Suitable for IoT beginners and embedded systems integration

---

## 🛠️ Tools and Libraries

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
