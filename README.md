## ESP32 Room Data Dashboard

A real-time environmental monitoring system that collects data from an ESP32 and displays it on an interactive web dashboard hosted via GitHub Pages.

### 🌐 Live Demo
You can view the live dashboard [here](https://alecava01.github.io/ESP32-room-data-dashboard/)

### 🛠️ How It Works
This project utilizes a serverless architecture to ensure 24/7 availability with zero hosting costs:

Hardware (ESP32): Reads environmental data (Temperature, Humidity, Pressure) and sends an HTTP GET request to a Google Apps Script.

Database (Google Sheets): The Google Apps Script receives the parameters and appends them as a new row in a spreadsheet.

Backend (Google Apps Script): Acts as a REST API, processing incoming hardware data and serving the historical data as a JSON string.

Frontend (GitHub Pages): A Single Page Application (SPA) built with HTML5, Tailwind CSS, and Chart.js. It fetches data from the Google Script every 5 seconds to update the visuals dynamically.