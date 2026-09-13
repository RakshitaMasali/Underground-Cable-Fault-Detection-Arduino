# Underground-Cable-Fault-Detection-Arduino
Arduino-based underground cable fault detection and distance estimation system using voltage sensing, relays, LCD and buzzer.
# Underground Cable Fault Detection using Arduino

An Arduino-based prototype for detecting and estimating the approximate location of faults in underground cable sections using voltage sensing, relays, an LCD display, and a buzzer.

## 📌 Project Overview

Underground cable faults such as short circuits, open circuits, and insulation-related faults can be difficult to locate because the cables are buried underground.

This project demonstrates a low-cost **Arduino-based underground cable fault detection and localization system**. The system monitors voltage variations using an analog sensor and uses relay-controlled cable sections to simulate different fault locations.

When a fault is detected, the system:

* Identifies the affected cable section
* Estimates the approximate fault distance
* Displays the result on a 16×2 LCD
* Activates a buzzer as an audible alert

> **Note:** This is an educational prototype/simulation. The distance calculation is approximate and is intended for demonstration rather than industrial cable fault localization.

## 🎯 Objectives

* Detect abnormal voltage conditions indicating a cable fault
* Estimate the approximate distance of the fault
* Display fault status on a 16×2 LCD
* Provide an audible fault alert using a buzzer
* Simulate different underground cable sections using relays
* Develop a low-cost and easy-to-understand fault detection prototype

## ⚙️ Working Principle

1. The Arduino initializes the LCD, analog sensor, relays, and buzzer.
2. The relays are activated one at a time to simulate different cable sections.
3. The analog sensor reads the voltage condition of the selected section.
4. The Arduino processes the analog reading and calculates an approximate distance.
5. If a fault is detected, the distance is displayed on the LCD and the buzzer is activated.
6. If no fault is detected, the LCD displays **NF (No Fault)**.
7. The process continuously repeats for real-time monitoring.

### Distance Calculation

```text
Distance = ADC Value / 100
```

The calculated value is used as an **approximate demonstration distance in kilometres**.

## 🔧 Hardware Components

* Arduino UNO
* Analog voltage sensing circuit / resistor network
* Relay modules
* ULN2003 relay driver IC

