# 🌦️ Weather API QA Suite

## 📌 Project Overview
This project is a **QA Automation Test Suite** for validating a Weather API system.

It tests:
- Geocoding API (City → Coordinates)
- Weather API (Coordinates → Weather Data)
- End-to-End Flow (City → Weather)

---

## 🧪 Test Scenarios

### 1. Geocoding Tests
- ✅ Valid City → Returns coordinates
- ❌ Invalid City → Returns empty response

### 2. Weather Tests
- ✅ Valid Coordinates → Returns weather data

### 3. End-to-End Flow
- 🔄 City → Coordinates → Weather

---

## 🔗 APIs Used

### Geocoding API

https://nominatim.openstreetmap.org/search?q={{city}}&format=json


### Weather API

https://api.open-meteo.com/v1/forecast?latitude={{lat}}&longitude={{lon}}&current_weather=true


---

## ⚙️ Environment Variables

| Variable | Description |
|----------|------------|
| city     | Input city |
| lat      | Latitude |
| lon      | Longitude |

---

## ▶️ How to Run

### Using Postman
1. Import Collection
2. Import Environment
3. Select Environment
4. Click **Runner**
5. Run Collection

---

## 📊 Sample Test Validations

- Status code = 200
- Response is array (Geocoding)
- Latitude & Longitude extracted
- Weather data exists
- Temperature field present

---

## 📸 Test Results

(All tests passed successfully)

---

## 🛠 Tools Used
- Postman
- Open-Meteo API
- OpenStreetMap Nominatim API

---

## 👨‍💻 Author
Priyanshu Solon
