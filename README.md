# 🌱 Smart Crop Monitoring System

### ESP32-Based Smart Irrigation and Crop Monitoring System

An IoT-based smart agriculture system that monitors soil moisture and water usage and automates irrigation using an ESP32, Real-Time Clock (RTC), soil moisture sensor, digital flow meter, water pump, keypad, and LCD display.

---

## 📌 Overview

The Smart Crop Monitoring System is designed to improve irrigation efficiency by continuously monitoring soil moisture and controlling water delivery based on crop requirements.

The system uses an ESP32 as the main controller. A VH400 soil moisture sensor monitors the moisture level of the soil, while a Real-Time Clock (RTC) provides accurate timing for scheduled irrigation.

A digital flow meter measures the water flow during irrigation. The ESP32 processes the sensor information and controls the water pump according to the required irrigation conditions.

The system also includes an LCD display and keypad for user interaction, monitoring, and configuration. The ESP32's built-in Wi-Fi capability enables cloud connectivity for remote monitoring and control.

---

## 🎯 Objectives

- Monitor soil moisture in real time.
- Automate irrigation based on soil moisture conditions.
- Schedule irrigation using a Real-Time Clock.
- Measure water flow and water usage.
- Reduce water wastage.
- Reduce the need for manual irrigation.
- Provide real-time information through an LCD display.
- Enable remote monitoring through cloud connectivity.
- Improve irrigation efficiency and promote sustainable agriculture.

---

## 🔧 Hardware Components

- ESP32 Microcontroller
- VH400 Soil Moisture Sensor
- Real-Time Clock (RTC)
- Digital Flow Meter
- Water Pump
- Keypad
- LCD Display
- Power Supply
- DC Motor

---

## 💻 Technologies Used

- ESP32
- IoT
- Embedded Systems
- Soil Moisture Monitoring
- Real-Time Clock
- Cloud Connectivity
- Sensor Integration
- Automated Irrigation
- Wi-Fi

---

## 🏗️ System Architecture

The main controller of the system is the ESP32.

### Inputs

- Soil Moisture Sensor (VH400)
- Real-Time Clock
- Digital Flow Meter
- Keypad

### Processing

- ESP32 Microcontroller

### Outputs

- Water Pump
- LCD Display
- Cloud Monitoring

The block diagram in the project report shows the ESP32 receiving information from the soil moisture sensor, RTC, and digital flow meter, while controlling the water pump/keypad and LCD display.

---

## ⚙️ Working Principle

### Step 1: Soil Moisture Sensing

The VH400 soil moisture sensor continuously monitors the moisture level in the soil and provides a signal representing the current soil condition.

### Step 2: Data Processing

The ESP32 receives the sensor information and compares the soil moisture condition with the required moisture threshold.

### Step 3: Irrigation Control

When the soil moisture falls below the required level, the ESP32 activates the water pump to begin irrigation.

### Step 4: Water Flow Monitoring

The digital flow meter measures the water flow during irrigation and allows the system to monitor the amount of water being delivered.

### Step 5: Irrigation Scheduling

The RTC provides accurate time and date information. This allows irrigation events to be scheduled according to user-defined timing.

### Step 6: User Interaction

The keypad allows the user to manually control the system, set irrigation schedules, and adjust parameters.

The LCD displays information such as:

- Soil moisture level
- Current time
- Water flow rate
- Total water usage
- System status

### Step 7: Cloud Connectivity

The ESP32's built-in Wi-Fi capability enables sensor information to be transmitted to a cloud platform for remote monitoring and control.

---

## 🔄 Overall Workflow

```text
        Soil Moisture Sensor
                │
                ▼
        ┌───────────────┐
        │     ESP32     │
        └───────┬───────┘
                │
       ┌────────┼─────────┐
       │        │         │
       ▼        ▼         ▼
   Water Pump  LCD      Cloud
       │      Display   Monitoring
       │
       ▼
   Irrigation

RTC ──────────► ESP32
Flow Meter ───► ESP32
Keypad ───────► ESP32
