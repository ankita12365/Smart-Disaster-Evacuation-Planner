# 🌍 Smart Disaster Evacuation Planner

Smart Disaster Evacuation Planner is a web-based IoT disaster management system that calculates the **safest evacuation route between cities** using real-time disaster risk data collected from ESP32 sensors.

The system uses a **risk-weighted Dijkstra Algorithm** to analyze distance and disaster conditions, then displays the safest possible route on an interactive map interface.

The project is demonstrated using the **Uttarakhand region map** with cities like Haridwar, Dehradun, Rishikesh, Mussoorie, and other locations.

---

# 🚀 Features

- 🌐 Real-time disaster risk data from ESP32
- 🛣️ Safest route calculation using Weighted Dijkstra Algorithm
- 🗺️ Interactive map visualization
- 📍 Highlighted evacuation path
- 📊 Live disaster risk updates
- 🔌 Serial communication using Web Serial API
- 🎨 Color-coded disaster risk levels
- 🏙️ City-based source and destination selection
- ⚡ Lightweight and responsive web interface

---

# 🛠️ Technologies Used

## Frontend

- HTML5
- CSS3
- JavaScript

## Visualization

- D3.js (Map Visualization)

## Hardware & Communication

- ESP32 Development Board
- Web Serial API

## Sensors Used

- Water Level Sensor
- Vibration Sensor
- Flame Sensor
- DHT11 / DHT22 Temperature & Humidity Sensor

## Algorithm

- Dijkstra's Algorithm
- Weighted Graph Algorithm

---

# 📂 Project Structure

```text
Smart-Disaster-Evacuation-Planner/

│
├── images/
│   ├── Chamba.jpg
│   ├── Default.jpg
│   ├── Dehradun.jpg
│   ├── Haridwar.jpg
│   ├── Mussoorie.jpg
│   ├── Rishikesh.jpg
│   └── Tehri.jpg
│
├── index.html
├── serial.js
├── esp32code.ino
├── package.json
├── package-lock.json
├── .gitignore
└── README.md
```

---

# ⚙️ Installation & Setup

## 1. Clone Repository

```bash
git clone https://github.com/ankita12365/Smart-Disaster-Evacuation-Planner.git
```

Navigate to project folder:

```bash
cd Smart-Disaster-Evacuation-Planner
```

---

## 2. Install Dependencies

```bash
npm install
```

---

## 3. Run the Project

Open:

```text
index.html
```

directly in your browser.

OR run using local server:

```bash
npx http-server
```

---

# 🔌 ESP32 Setup

1. Connect ESP32 board using USB cable
2. Upload `esp32code.ino`
3. Open the web application
4. Click on **Connect Serial**
5. ESP32 sends live disaster information

Example data format:

```json
{
  "city": "Haridwar",
  "flood": 2,
  "fire": 1,
  "vibration": 0
}
```

---

# 🧠 How It Works

1. User selects source and destination cities
2. ESP32 collects real-time sensor values
3. Data is transmitted through Web Serial API
4. Disaster risk values update the graph weights
5. Weighted Dijkstra Algorithm calculates the safest route
6. The map displays the recommended evacuation path

---

# 🔬 Algorithm Used — Dijkstra Algorithm

The project uses a modified Dijkstra Algorithm for safe route calculation.

### Graph Representation

- City → Node
- Road → Edge
- Edge Weight → Distance + Disaster Risk

The algorithm finds the path with the minimum combined risk and distance.

---

# 🔧 Hardware Components

- ESP32 Dev Board
- Water Sensor
- Vibration Sensor
- Flame Sensor
- DHT11/DHT22 Sensor
- Jumper Wires
- USB Cable

---

# 🎯 Applications

- Disaster evacuation planning
- Emergency route management
- IoT-based safety systems
- Smart city disaster response

---

# 🔮 Future Improvements

- GPS-based live tracking
- AI-based disaster prediction
- Weather API integration
- Google Maps integration
- Cloud database for risk history
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

⭐ An IoT + Algorithm-based solution for intelligent disaster evacuation planning.
