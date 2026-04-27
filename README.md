# 🚨 Rapid Crisis Response System (RCRS)
A real-time emergency coordination platform designed to streamline communication and evacuation guidance during building-level crises.

---

## 🧩 Problem Statement
In large-scale environments such as malls, corporate offices, and university campuses, emergency response is often hindered by:
* ⏳ **Delayed communication** between departments.
* ⚠️ **Conflicting instructions** causing public panic.
* 🌑 **Zero real-time visibility** for building managers.
* 📉 **Fragmented coordination** between staff, guests, and rescue teams.

This gap in communication leads to stairwell congestion, slower evacuations, and increased risk to human life.

## 💡 Solution Overview
**RCRS** provides a centralized, high-speed ecosystem where data flows vertically and horizontally in real-time:
* **Command & Control:** Managers verify threats and activate global alerts.
* **Operational Intelligence:** Security and staff receive live instructions.
* **Public Guidance:** Guests and digital screens receive floor-specific evacuation routes.
* **Tactical Support:** External rescue teams receive precise incident location data.

---

## ☁️ Google Technologies Used

### 1️⃣ Firebase Realtime Database
The "Nervous System" of RCRS. It handles:
* **State Synchronization:** Sub-100ms updates across all connected clients.
* **Dynamic Routing:** Real-time logic for "Safe" vs "Blocked" exit status.
* **Concurrency:** Managing simultaneous reports from multiple staff wardens.

### 2️⃣ Firebase Hosting
Provides a secure, global SSL-encrypted hosting environment, ensuring the dashboards are accessible on any mobile or desktop device instantly during a crisis.

### 3️⃣ Google Maps Platform
Integrated via the Embed API to provide:
* **Spatial Awareness:** Visualizing "Site Alpha" incident locations.
* **Logistics Coordination:** Helping rescue teams identify the correct access gates.

---

## 🧠 Technical Architecture

```mermaid
graph TD
    A[Manager Dashboard] -->|Write Event| B(Firebase Realtime DB)
    B -->|Sync Status| C[Guest/Staff View]
    B -->|Sync Status| D[Public Screen]
    B -->|Sync Status| E[Rescue Tactical View]
    C -->|Report Incident| B

## 🚀 Live Prototype
The system is fully deployed on Google Firebase. You can access the different modules via the links below:

### 🔗 Hosted Application:
* **Manager Dashboard:** [Launch Manager](https://rapidcrisisresponse-b7231.web.app/manager.html)
* **Staff Interface:** [Launch Staff](https://rapidcrisisresponse-b7231.web.app/staff.html)
* **Security Terminal:** [Launch Security](https://rapidcrisisresponse-b7231.web.app/security.html)
* **Rescue Team View:** [Launch Rescue](https://rapidcrisisresponse-b7231.web.app/rescue.html)
* **Guest Reporter:** [Launch Guest](https://rapidcrisisresponse-b7231.web.app/guest.html)
* **Public Display Screen:** [Launch Screen](https://rapidcrisisresponse-b7231.web.app/screen.html)

---

---

## 📁 Project Structure
* **`manager.html`** — Crisis activation and verification center.
* **`staff.html`** — Incident reporting and medical alerts.
* **`screen.html`** — Public-facing digital signage.
* **`rescue.html`** — External agency tactical overview.
* **`security.html`** — Building-wide status monitor.
* **`guest.html`** — Public reporting interface.

---

## 🌱 Future Scope
* **AI Integration:** Using **Gemini** to calculate optimal evacuation paths based on real-time crowd density and obstacle data.
* **IoT Connectivity:** Implementing automatic crisis triggers via smart smoke, heat, and structural vibration sensors.
* **Multilingual Support:** Instant AI-driven translation of safety instructions to assist diverse populations in public spaces.

---
