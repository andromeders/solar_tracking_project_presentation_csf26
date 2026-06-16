# 🛰️ Dual-Axis Solar Tracker Project — Operation Green Energy 2026

[![Andromeders Ecosystem](https://img.shields.io/badge/Ecosystem-Andromeders-CCFF00?style=for-the-badge)](https://andromeders.com)
[![Target Audience](https://img.shields.io/badge/Generation-Next%20Genius%20Generation-00E5FF?style=for-the-badge)]()
[![Platform](https://img.shields.io/badge/Platform-Arduino%20R3-purple?style=for-the-badge)]()

Welcome to the official repository of the **Dual-Axis Solar Tracker Project**, an advanced STEM and social innovation initiative developed under the **Andromeders** framework. This project empowers the *Next Genius Generation* (students aged 11 to 14) to bridge the gap between software engineering, mechanical assembly, and renewable energy.

Inspired by Morocco's world-class renewable energy infrastructure—such as the **Noor Ouarzazate Solar Complex**—this project challenges students to maximize solar panel efficiency by building an autonomous system that tracks light in real-time across a 180-degree field.

---

## 📋 Project Overview

A standard fixed solar panel loses up to **40% of potential energy** daily simply because it faces only one direction. This project solves that problem. By leveraging a custom-built hardware frame and an algorithmic feedback loop, our smart tracker dynamically adjusts its position to harvest maximum photons, demonstrating a **+25% increase in energy efficiency** during live benchmarking.

This repository contains the complete technical ecosystem, including:
* Embedded source code (C/C++ Arduino sketches)
* Circuit wiring schematics and pin mapping
* System architecture and algorithmic flowcharts

---

## 🧠 System Architecture & Hardware Inventory

The prototype is structured like a living organism, balancing mechanics, electronics, and logic:

* **The Brain:** Arduino R3 microcontroller + V5.0 Sensor Shield for centralized calculation and data processing.
* **The Eyes:** 4 Photoresistors (LDRs) calibrated in a directional cross-configuration to track light intensity from four quadrants (Left, Right, Up, Down).
* **The Muscles:** 2 SG90 Servo Motors managing dual-axis rotation:
  * **Azimuth Axis:** Horizontal tracking (East to West rotation).
  * **Pitch Axis:** Vertical tracking (Sun altitude adaptation).
* **Power & Metrics:** 10650 Shield & Charge Detector paired with a USB Charge Detector to live-stream voltage and output variations.

---

## 💻 The "Search" Algorithm Logics

The core software operates on a continuous, zero-error feedback loop (`void loop()`) that ensures equilibrium:

1. **Scan:** The microcontroller constantly reads analog voltage values from the 4 LDR sensors.
2. **Compare:** The software calculates the differential between opposite pairs (e.g., `Left_LDR` vs. `Right_LDR`).
3. **Correct:** If an imbalance is detected, the corresponding servo motor increments its position toward the brighter source until the difference is minimized to zero.

---

## 👥 Engineering Cell Roles

To succeed in the final **Solar Performance Gala**, students operate in specialized engineering cells with dedicated responsibilities:
* **Project Leader:** Coordinates milestones, drives social innovation alignment, and presents global climate impacts.
* **Hardware Engineer:** Oversees laser-cut acrylic frame assembly and optimizes mechanical tolerances (brass standoffs).
* **Software Architect:** Calibrates threshold tolerances, maps sensor pins, and programs the automated tracking logic.
* **Data Analyst:** Tracks real-world efficiency gains using the USB monitor during the "Blackout Test Scenario".

---

## 📂 Core Reference Documentation

For deep-dive methodology, pedagogical pathways, and operational parameters, please refer to our internal master files:
* `NOTE DE CADRAGE - SOLAR TRACKING PROJECT.pdf` — Project charter, vision, and strategic framing.
* `FEUILLE DE ROUTE PÉDAGOGIQUE ET TECHNIQUE - SOLAR TRACKING PROJECT.pdf` — Session-by-session technical and pedagogical roadmap.
* `STUDENT MISSION BRIEF - SOLAR TRACKING PROJJECT.pdf` — Mission instructions, role descriptions, and gala guidelines for the teams.
* `SOLAR TRACKING ROADMAP.jpeg` — Visual system architecture blueprint and hardware layout.

---

⚡ *Developed with passion by ANDROMEDERS. Unleashing collective intelligence to inspire humanity to achieve its full potential.*
