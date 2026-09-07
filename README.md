# Design and Implementation of Battery Optimization System Using SoC Estimation and Passive Cell Balancing

An ESP32-based embedded Battery Management System (BMS) for a 4S (16V nominal) Lithium-ion battery pack[span_0](start_span)[span_0](end_span). The system features high-precision 16-bit voltage sensing via ADS1115, current monitoring using INA219, hybrid State of Charge (SoC) estimation, and passive cell balancing via MOSFET-switched shunt resistors[span_1](start_span)[span_1](end_span).

📄 **[View Full Project Report (PDF)](./report/Project_Report.pdf)**

---

## 📸 Project Visuals & Hardware

### 📐 System Block Diagram
![Block Diagram](./block-diagram.jpeg)

### 🔌 Circuit Schematic
![Circuit Diagram](./circuit-diagram.jpeg)

### 🛠️ Hardware Prototype
![Hardware Setup](./hardware-setup.jpeg)

### 📺 OLED / Display Output Result
![Display Result](./lcd-display-result.jpeg)

---

## ⚡ Key Features
* **16-Bit Sensing:** Uses ADS1115 ADC with resistor divider network for per-cell monitoring[span_2](start_span)[span_2](end_span).
* **Passive Cell Balancing:** Dissipates extra charge via $47\Omega$ shunt resistors using IRLZ44N MOSFET switches[span_3](start_span)[span_3](end_span).
* **Protection Cutoff:** Disconnects load via relay when any cell drops below 3.0V[span_4](start_span)[span_4](end_span).

---

## 💻 Firmware Code
The full source code is available in [`src/BMS_Control.ino`](./src/BMS_Control.ino)[span_5](start_span)[span_5](end_span).

---

## 👥 Authors & Group Details
* **Group No:** 03[span_6](start_span)[span_6](end_span)
* **Members:** Ritesh Gade, Manan Shah, Khushal Tumma, Aadi Vora[span_7](start_span)[span_7](end_span)
* **Guide:** Dr. Shruti Nema[span_8](start_span)[span_8](end_span)
* **Department:** Electrical Engineering, Lokmanya Tilak College of Engineering[span_9](start_span)[span_9](end_span)
*
