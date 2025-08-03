# 🌿 IoT Smart Plant Monitoring & AI-Based Disease Detection 
This project combines IoT automation and AI image classification to ensure efficient plant care and early disease detection.

🔧 Technologies Used
ESP8266/NodeMCU

Blynk IoT App

Soil Moisture + DHT11 Sensor

Python + TensorFlow + Streamlit

Docker

# 📦 Project Features
🛰 IoT Plant Monitoring
Live soil moisture, temperature, and humidity data

Automated irrigation via solenoid valve

Manual override and alerts using Blynk app

# 🧠 AI Disease Detection
CNN-based image classifier for plant disease detection

Simple web interface using Streamlit

Dockerized for easy deployment

# 🛠️ Setup Instructions
🔌 1. IoT Monitoring System (Hardware + Blynk)
📋 Required Components
ESP8266 (NodeMCU)

Soil Moisture Sensor

DHT11/DHT22 Sensor

Relay Module + Solenoid Valve

Jumper wires, Breadboard, Power Supply

# 🧾 Steps:
Connect sensors to NodeMCU as per circuit diagram (see /hardware folder).

Flash esp8266_code.ino using Arduino IDE.

Install Blynk on your phone.

Create a new project and:

Add widgets for moisture, temp, humidity

Add a button for controlling the solenoid

Link ESP8266 to Wi-Fi and Blynk Auth Token.

# 🧠 2. AI-Based Disease Detection (Web App)
📋 Requirements
Python 3.10+

Docker (optional)

Dependencies listed in requirements.txt

# 🚀 Run Without Docker
# Clone the repo
git clone https://github.com/YOUR-USERNAME/iot-plant-monitoring-ai.git
cd iot-plant-monitoring-ai/software/streamlit_app

# Install dependencies
pip install -r requirements.txt

# Start the Streamlit app
streamlit run app.py

# Clone the repo
git clone https://github.com/YOUR-USERNAME/iot-plant-monitoring-ai.git
cd iot-plant-monitoring-ai/software/streamlit_app

# Install dependencies
pip install -r requirements.txt

# Start the Streamlit app
streamlit run app.py
🐳 Run With Docker
bash
Copy
Edit
# Build Docker image
docker build -t plant-disease-app .

# Run container
docker run -p 8501:8501 plant-disease-app
Visit: http://localhost:8501
