# 🚀 Water Quality Monitoring App (React Native + LoRa)

A simple mobile app built with **React Native** to display real-time water quality data collected from an embedded system using **ESP32 T-Beam + LoRa**.

The app connects to a database and shows the latest sensor readings (pH and temperature), along with historical data and technical metrics from the communication layer.

---

# 📌 Summary

* 📱 React Native app
* 📡 LoRa communication
* 🌊 Water quality monitoring
* ⚡ Real-time + historical data


# 📱 App Overview

## 🔐 Login Screen

Clean and simple authentication screen to validate users before accessing the app.

<p align="center">
  <img src="https://github.com/user-attachments/assets/d18ea9b3-04fc-48ec-a338-f01263c6d9a3" width="120" />
</p>

---

## 🏠 Home Screen

Displays the **latest data received** from the database.

* Uses real-time updates
* Fetches the most recent child node
* Focus on up-to-date information

<p align="center">
  <img src="https://github.com/user-attachments/assets/9ee847c8-68e9-4719-9721-da595776b5ee" width="120" />
</p>

---

## 📊 History Screen

Shows **all recorded data** from the database.

* Lists historical sensor readings
* Useful for tracking trends
* Based on full node retrieval

<p align="center">
  <img src="https://github.com/user-attachments/assets/e38a7c75-5362-46bd-ba5b-1e827e755ab0" width="120" />
</p>

---

## 📡 Technical Screen

Displays LoRa communication metrics:

* 📶 RSSI (signal strength)
* 📉 SNR (signal-to-noise ratio)
* 📦 Packet loss

<p align="center">
  <img src="https://github.com/user-attachments/assets/c127346d-32be-43e6-81f3-fc20d8fc6c5b" width="120" />
</p>

---

## ⚙️ Settings Screen

Basic user and app information.

* Logged-in user details
* Data description
* Simple configuration options

<p align="center">
  <img src="https://github.com/user-attachments/assets/467f8684-b5e1-429f-b8c1-0fe96633ca05" width="120" />
</p>

---

# 🌊 Embedded System (LoRa)

This app integrates with a **water quality monitoring system**.

* Sensors collect environmental data
* ESP32 transmits via LoRa
* Receiver processes and stores data

🔗 Receiver repository:
[https://github.com/ndamasc/Esp-Receiver-Lora](https://github.com/ndamasc/Esp-Receiver-Lora)

---

# 🧰 Hardware

* **PH4502C** → pH measurement
* **DS18B20** → Temperature sensor
* **ESP32 T-Beam** → Microcontroller
* **LoRa module** → Long-range communication

---

# 🛠 Requirements

* ESP32 T-Beam (2 units)
* PH4502C sensor
* DS18B20 sensor
* Resistors: 1KΩ, 2KΩ, 4.7KΩ
* LoRa Library (Sandeep)
* VS Code (or compatible IDE)

---

# ⚙️ How It Works

1. Sensors collect pH and temperature
2. ESP32 processes the data
3. Data is transmitted via LoRa
4. ESP32 Receiver stores/processes data
5. Mobile app displays the information

Extra metrics collected:

* RSSI
* SNR
* Packet loss

---

# 📂 Project Structure

* **Readings** → Sensor data acquisition
* **LoRa Communication** → Data transmission
* **Storage** → Backup if transmission fails

---

# 🔌 Circuit Diagram

<p align="center">
  <img src="https://github.com/user-attachments/assets/de97c8cb-4fde-4ede-be6c-89929403cf51" width="300" />
</p>

### ⚠️ Notes

* DS18B20 requires a **pull-up resistor (4.7KΩ)**
* Use **1KΩ + 2KΩ resistors** exactly as shown in the diagram

---

# 🚧 Improvements

Suggestions for future enhancements:

* Dissolved oxygen sensor
* Turbidity sensor
* Alerts/notifications
* Data analytics dashboard

---

