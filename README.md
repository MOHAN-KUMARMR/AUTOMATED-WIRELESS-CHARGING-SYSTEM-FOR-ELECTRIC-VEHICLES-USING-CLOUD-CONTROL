# Automated Wireless Charging System for Electric Vehicles Using Cloud Control

## Overview

The **Automated Wireless Charging System for Electric Vehicles (EVs) Using Cloud Control** is a smart charging system designed to enable wireless power transfer between a transmitter and receiver coil without requiring a physical charging cable.

The project integrates **inductive wireless power transfer, ESP32-based embedded control, ESP32-CAM-based vehicle alignment, and cloud-based monitoring** to support automated and remotely monitored EV charging.

The project combines simulation and hardware implementation to demonstrate the concept of automated wireless EV charging.

---

## Problem Statement

Conventional electric vehicle charging systems generally require a physical connection between the charging station and the vehicle.

This can create challenges such as:

* Manual connection and disconnection of charging cables
* Requirement for accurate vehicle positioning
* Cable handling and maintenance
* Limited charging automation
* Difficulty in remotely monitoring the charging process

To address these challenges, this project proposes an **automated wireless charging system** that transfers electrical power between transmitter and receiver coils through inductive coupling.

---

## Objectives

The main objectives of this project are:

* To develop a wireless charging system for electric vehicles.
* To demonstrate electrical power transfer using **inductive wireless power transfer (WPT)**.
* To automate the charging process.
* To assist with vehicle positioning and coil alignment.
* To integrate ESP32-based embedded control.
* To use ESP32-CAM for vehicle alignment and direction indication.
* To provide cloud-based monitoring of charging/system status.
* To demonstrate a smart and remotely monitored EV charging solution.

---

## System Architecture

The system consists of the following major functional blocks:

```text
                     ELECTRIC VEHICLE
                            │
                            ▼
                  Vehicle Detection /
                    Alignment System
                            │
                            ▼
                         ESP32
                     ┌──────┴──────┐
                     │             │
                     ▼             ▼
              Charging Control   Cloud Monitoring
                     │             │
                     ▼             ▼
              Transmitter Coil   Remote Monitoring
                     │
                     │
              Wireless Power
                 Transfer
                     │
                     ▼
                 Receiver Coil
                     │
                     ▼
                  EV Battery
```

The transmitter and receiver coils form the wireless power transfer path. The ESP32 manages embedded control and monitoring functions, while the ESP32-CAM assists with vehicle alignment and direction indication.

---

## Hardware Components

The prototype uses the following major hardware components:

| Component        | Purpose                                    |
| ---------------- | ------------------------------------------ |
| ESP32            | Embedded control and system communication  |
| ESP32-CAM        | Vehicle alignment and direction monitoring |
| Transmitter Coil | Wireless power transmission                |
| Receiver Coil    | Wireless power reception                   |
| Power Supply     | Provides electrical power to the system    |
| Sensors          | Vehicle/system detection and monitoring    |
| Battery / Load   | Receives transferred electrical power      |

---

## Software / Technologies

### Embedded Systems

* ESP32
* ESP32-CAM
* Embedded programming
* Camera-based monitoring

### Wireless Power Transfer

* Inductive Wireless Power Transfer (WPT)
* Transmitter and receiver coil system
* Power transfer simulation

### Cloud

* Cloud-based monitoring
* Real-time charging/system status monitoring

### Programming

* C/C++ for ESP32 development

---

## Working Principle

The system operates through the following stages.

### 1. Vehicle Positioning

The electric vehicle is positioned over the wireless charging area.

The alignment system assists in determining the vehicle position relative to the wireless charging coils.

### 2. Vehicle Alignment

The **ESP32-CAM** is used to assist with vehicle alignment and direction indication.

Proper alignment between the transmitter and receiver coils is important for effective wireless power transfer.

### 3. Wireless Power Transfer

Once the vehicle is appropriately positioned, electrical power is transferred from the transmitter coil to the receiver coil through **inductive wireless power transfer**.

### 4. Charging

The electrical power received through the receiver side is supplied to the connected battery/load.

### 5. Cloud Monitoring

The system provides cloud-based monitoring of the charging/system status, enabling remote observation of the system.

### 6. Automated Control

The ESP32-based controller coordinates the monitoring and control functions of the system, reducing the need for manual intervention.

---

## Implementation

The project was implemented by integrating the following major subsystems.

### Wireless Charging Subsystem

The transmitter and receiver coils were used to demonstrate wireless power transfer between the charging and receiving sides.

### Embedded Control Subsystem

An **ESP32** was integrated to provide embedded control and system monitoring functions.

### Vehicle Alignment and Monitoring

An **ESP32-CAM** was integrated to assist with vehicle positioning, alignment, and direction indication.

### Cloud Monitoring

Cloud-based monitoring was integrated to provide real-time information regarding the charging/system status.

### WPT Simulation

A wireless power transfer model was developed and simulated to study the power transfer between the transmitting and receiving coils.

---

## Results

The developed project demonstrates the following capabilities:

* Wireless power transfer for EV charging
* Automated charging concept
* Vehicle alignment assistance
* ESP32-based embedded control
* ESP32-CAM-based monitoring
* Cloud-based charging/system monitoring
* WPT system simulation

### WPT Simulation Results

The wireless power transfer system was modeled and simulated to evaluate power transfer between the transmitting and receiving coils.

| Parameter                | Simulation Value |
| ------------------------ | ---------------: |
| Input Voltage            |        **240 V** |
| Target Output Voltage    |        **400 V** |
| WPT Power                |       **3.3 kW** |
| Simulated Output Voltage |     **≈407.9 V** |

The simulation demonstrates wireless power transfer through inductive coupling between the transmitter and receiver coils.


### Prototype Results

The physical prototype demonstrates:

* Wireless power transfer using transmitter and receiver coils
* ESP32-based embedded control
* ESP32-CAM-based vehicle alignment assistance
* Charging/system monitoring
* Cloud-based monitoring and control

---

## Simulation

The WPT simulation model was developed to evaluate the wireless power transfer system under the specified operating conditions.

### Simulation Parameters

```text
Input Voltage        : 240 V
Target Output Voltage: 400 V
WPT Power             : 3.3 kW
Simulated Output      : ≈407.9 V
```

The simulation output indicates that the system reaches approximately **407.9 V** on the receiving/output side for the modeled operating condition.

---

## Demo <img width="825" height="295" alt="image" src="https://github.com/user-attachments/assets/c0eba60c-f8f8-4f9f-8f9c-0ba3f035b514" />

**Demo:** <img width="1600" height="782" alt="WhatsApp Image 2026-08-14 at 1 47 57 PM" src="https://github.com/user-attachments/assets/d6e5a9ab-9ca9-4eaf-ad41-f7e2029096d7" />


**Demo Video:** `AUTOMATED WIRELESS CHARGING SYSTEM (1).mp4`

---

## IEEE Publication

This project has been published as an **IEEE research paper**.

**DOI:**

`10.1109/ICRISET64803.2025.11252334`

The publication is associated with the **Automated Wireless Charging System for Electric Vehicles** project.

---

## Future Improvements

Possible future improvements include:

* Improving wireless charging efficiency
* Optimizing transmitter and receiver coil alignment
* Increasing wireless charging power
* Improving automatic vehicle positioning
* Adding automatic charging start/stop control
* Improving cloud monitoring and data visualization
* Adding battery State of Charge (SOC) monitoring
* Improving system safety and fault detection
* Developing a larger-scale EV charging prototype
* Improving the wireless power transfer control system

---

## Project Highlights

### Key Technologies

`ESP32` `ESP32-CAM` `Wireless Power Transfer` `Cloud Monitoring` `Embedded Systems` `EV Charging`

### Key Features

* Wireless EV charging
* Inductive power transfer
* Vehicle alignment assistance
* ESP32-based control
* ESP32-CAM monitoring
* Cloud-based monitoring
* WPT simulation
* Physical prototype

---

## Author

### Mohan Kumar M R

**M.Tech — Electronics and Communication Engineering**
**PES University, Bengaluru**

### Areas of Interest

* VLSI
* Digital Electronics
* Embedded Systems
* Wireless Power Transfer
* Electric Vehicle Technology

---

## Repository Structure

```text
AUTOMATED-WIRELESS-CHARGING-SYSTEM-FOR-ELECTRIC-VEHICLES-USING-CLOUD-CONTROL/
│
├── README.md
├── AUTOMATED WIRELESS CHARGING SYSTEM (1).mp4
├── Project Images
└── Simulation / Documentation Files
```

---

## Publication

**IEEE Research Paper**

DOI: `10.1109/ICRISET64803.2025.11252334`

---

## Keywords

`Electric Vehicles` `Wireless Charging` `Wireless Power Transfer` `WPT` `ESP32` `ESP32-CAM` `Cloud Control` `Embedded Systems` `Inductive Power Transfer` `EV Charging`
