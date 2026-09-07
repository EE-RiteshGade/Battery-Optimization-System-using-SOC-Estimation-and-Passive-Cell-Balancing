# Design and Implementation of Battery Optimization System Using SoC Estimation and Passive Cell Balancing

An ESP32-based embedded Battery Management System (BMS) designed to monitor individual cell voltages, calculate State of Charge (SOC), perform passive cell balancing, and trigger safety protection using precision ADC and current sensing.

## Hardware Used
- ESP32 Microcontroller
- ADS1115 16-Bit ADC Module
- INA219 Current & Voltage Sensor Module
- IRLZ44N MOSFETs & Shunt Resistors (Passive Balancing)
- Protection Relay Module
- 0.96" OLED Display

## How It Works
The system continuously samples individual cell node voltages via the ADS1115 ADC and total pack current via the INA219 sensor. The ESP32 calculates individual cell voltages and overall State of Charge (SOC). When cell imbalance occurs during charging, the system engages MOSFET switches across shunt resistors to bleed excess charge from higher-voltage cells. If any cell falls outside safe operating limits (below 3.0V or above 4.2V), the protection relay instantly isolates the battery pack.

## Circuit Diagram

### Block Diagram:
![System Block Diagram](System%20Block%20Diagram.jpeg)

### Circuit Schematic:
![Circuit Schematic](Circuit%20Schematic.jpeg)

## Results

### Hardware Prototype:
![Hardware Prototype](Hardware%20Prototype.jpeg)

### OLED Display Telemetry Output:
![OLED Display Result](OLED%20Display%20Output%20Result.jpeg)

Validated across all per-cell sensing channels and load tests: the system accurately displays live per-cell voltages, total pack voltage, current, and SOC percentage while actively maintaining cell balance.

## Author
Ritesh Gade — Final Year Electrical Engineering, Lokmanya Tilak College of Engineering
