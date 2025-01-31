# Assignment - Internet of Things

## Overview

Hardware and sensors are constantly added to our lives. Sensors produce data that often needs to be collected and analyzed. Having a basic knowledge of IoT protocols opens many doors for exciting projects as a web developer.
This assignment focuses on analyzing IoT data and visualizing it on a web-based dashboard using a cloud platform. It aims to enhance your understanding of IoT data, API integration, and web-based data visualization.

## Description

You will receive data from **Temperature & Humidity** and **Total Volatile Organic Compounds (TVOC)** Sensor connected via a WiFi gateway to an MQTT broker. You need to subscribe to the MQTT broker, create a web interface for this data, and visualize it on a chart.

You can set up open-source tools to make collection, storage, and graphing such as **The TIG Stack (Telegraf, InfluxDB, and Grafana)** or explore alternative tools that align with your interests and expertise.

## Assignment Tasks

1. **Subscribe** to the provided MQTT broker to receive real-time data from the sensors:

   **MQTT broker details**:
   - `mqtt://cscloud7-148.lnu.se:1883`
   - User: `iotlab`
   - Pass: `iotlab`
   - Topic: `'data/sht30'` (Temperature and Humidity data). Additional topics (like TVOC) may be added.

   The data format is **JSON**.

2. **Analyze the incoming data**, which includes:
   - **Temperature and Humidity** readings
   - **TVOC levels**
   - **Timestamp** of each reading

---

## Choose Your Toolset

### Option 1: **Telegraf + InfluxDB + Grafana (TIG Stack)**
- **Telegraf**: Configure it to subscribe to the MQTT topic and collect data.
- **InfluxDB**: Store the incoming data in this time-series database.
- **Grafana**: Visualize the data on a dashboard with real-time charts and historical data.

### Option 2: **Node.js + MongoDB + Frontend Framework**
- **MongoDB**: Store the sensor data.
- **Node.js**: Use **MQTT.js** to subscribe to the MQTT broker and process the data into MongoDB.
- **Frontend Framework**: Build a custom web interface using **React.js**, **Next.js**, **Angular**, etc., with real-time charts using **Chart.js** or **D3.js**.

---

## Deliverables

### Functional Dashboard
- Provide a URL to a **functional dashboard** built using your selected toolset.

### Configuration Files
- **For TIG Stack**: Provide the **Telegraf configuration**, **InfluxDB setup**, and **Grafana dashboard export**.
- For **MongoDB**: Share the schema or structure of the database used for storing data.
- Share any **backend configuration** or scripts used.

### Documentation
- Explain the setup process for the toolset.
- Describe how data flows from the MQTT broker to the dashboard.
- Explain optimizations for handling time-series data.

---

## Merge Request

Submit the assignment by creating a **Merge Request** to the `lnu/submit-branch`. It's acceptable to include additional projects or repositories, but include links to them in the submission report.

Don't forget to include a link to your **Assignment Report**.

---

## Learning Outcomes

By completing this assignment, you will:

- Understand how to collect real-time data using MQTT.
- Learn how to store and manage IoT data efficiently.
- Gain hands-on experience with professional IoT tools.
- Develop skills in creating dashboards and visualizing sensor data.
