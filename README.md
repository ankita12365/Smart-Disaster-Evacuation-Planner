# 🌍 Smart Disaster Evacuation Planner

Smart Disaster Evacuation Planner is a web-based disaster management system that calculates the safest evacuation route between cities using real-time disaster risk data received from hardware sensors.

The system combines **real-time ESP32 sensor data**, **weighted Dijkstra's Algorithm**, and **interactive map visualization** to find the safest and shortest possible route during disaster situations.

The project was demonstrated using the **Uttarakhand map** as a disaster simulation environment.

---

# 🚀 Features

- 🌐 Real-time disaster risk data collection using ESP32
- 🛣️ Safest path calculation using Weighted Dijkstra Algorithm
- 🗺️ Interactive map visualization with highlighted safe routes
- 📊 Live disaster risk table updates
- 🔌 Serial communication using Web Serial API
- 📍 Start and destination city selection
- 🎨 Color-coded disaster risk levels
- ⚡ Lightweight and responsive frontend interface

---

# 🛠️ Technologies Used

## Frontend
- HTML
- CSS
- JavaScript

## Visualization
- D3.js (Map Visualization)

## Hardware & Communication
- ESP32 Development Board
- Web Serial API

## Algorithm
- Dijkstra's Algorithm

## Sensors Used
- Water Level Sensor
- Vibration Sensor
- Flame Sensor
- DHT11 / DHT22 Temperature & Humidity Sensor

---

# 📂 Project Structure

```text
Smart-Disaster-Planner/

│
├── index.html
├── serial.js
├── esp32code.ino
├── README.md
```

---

# ⚙️ Installation & Setup

## 1. Run the Project

Clone the repository:

```bash
git clone https://github.com/ankita12365/Smart-Disaster-Evacuation-Planner.git
```

Open the project folder:

```bash
cd Smart-Disaster-Evacuation-Planner
```

Run the application:

Option 1:
- Open `index.html` directly in your browser

Option 2:
Run using local server:

```bash
npx http-server
```

---

# 🔌 ESP32 Setup

1. Connect ESP32 board using USB cable
2. Upload `esp32code.ino` to ESP32
3. Open the webpage
4. Click on **Connect Serial**
5. ESP32 starts sending live disaster data

Example JSON format:

```json
{
  "Haridwar": {
    "flood": 2,
    "fire": 1,
    "vibration": 0
  }
}
```

---

# 🧠 How It Works

1. User selects source and destination cities
2. ESP32 collects real-time disaster sensor values
3. Sensor data is transmitted through Web Serial API
4. System updates the risk-weighted graph
5. Weighted Dijkstra Algorithm calculates the safest route
6. The map highlights the recommended evacuation path

---

# 🔬 Algorithm Used — Dijkstra Algorithm

The project uses a modified version of Dijkstra's Algorithm.

### Graph Representation

- Each city → Node
- Each road → Edge
- Edge weight → Distance + Disaster Risk

### Output

The algorithm finds the path with the minimum combined risk and distance.

Dijkstra Algorithm is used because it is:
- Fast
- Reliable
- Efficient for shortest/safest path calculations

---

# 🔧 Hardware Setup

## Components

- ESP32 Development Board
- Water Sensor
- Vibration Sensor
- Flame Sensor
- DHT11/DHT22 Sensor
- Jumper Wires
- USB Cable

ESP32 sends disaster data through Serial communication:

```json
{
 "city":"Haridwar",
 "flood":2,
 "fire":1
}
```

---

# 🔮 Future Improvements

- GPS-based live location tracking
- AI-based disaster prediction
- Weather API integration
- Google Maps integration
- Cloud database for storing disaster history
- Mobile application support

---

# 👩‍💻 Contributors

- Riddhi Chopda
- Ankita Chavan
- Palak Chandak
- Bhumika Chaure

---

# 👩‍🏫 Guided By

**Prof. Rakhi Bharadwaj**

---

⭐ This project focuses on combining IoT, algorithms, and web technologies to create an intelligent disaster evacuation support system.
