#IoT-Based LPG Gas Leak Detection & Automatic Cut-Off System
Problem Statement:

In most Indian households, LPG cylinders are used for daily cooking. Gas leakage, faulty regulators, or accidentally leaving the stove ON can lead to serious accidents such as fire, explosions, or health hazards.
Existing safety methods mainly rely on human attention and local alarms, which may fail when users are not present at home.

Proposed Solution: 
We propose an IoT-based smart LPG gas safety system that continuously monitors gas levels near the stove or regulator area and automatically reacts in case of danger.

The system:
Detects LPG gas leakage using a gas sensor
Provides instant local alerts (buzzer & LED)
Uses a controller-based decision logic
Simulates automatic gas cut-off
Is designed as a non-invasive external add-on, without modifying government-issued LPG regulators

Hardware Components Used:
ESP32 Development Board
MQ-5 Gas Sensor
Active Buzzer
LED with resistor
Breadboard
Jumper wires
USB power supply
(Servo / solenoid valve planned for next round)

System Architecture & Working:
The gas sensor continuously measures gas concentration.
The ESP32 reads the analog sensor value.
The value is compared with a predefined safety threshold.
If gas concentration is below threshold:
System remains in monitoring state.
If gas concentration exceeds threshold:
Buzzer and LED are activated
Gas cut-off logic is triggered (simulated)
Alert message is generated

Prototype Status (Round-1 Submission):
Gas detection using MQ sensor is functional
ESP32 successfully processes sensor data
Buzzer and LED alert system works correctly
Gas cut-off is logically implemented (simulated)
Serial Monitor used for real-time monitoring and alerts
This prototype demonstrates the core functionality and feasibility of the system.

Planned Enhancements (Round-2 Scope):
In the next stage, the system will be enhanced with:
Physical gas cut-off using servo motor or solenoid valve
Compact clip-on enclosure compatible with LPG regulators
Mobile notification using IoT platform (Blynk/Firebase)
Improved false-alarm filtering
Battery backup for power failure
Multiple sensor placement for better coverage

Safety & Ethics Consideration:
The system is designed as an external safety attachment
It does not replace or modify government-issued LPG regulators  
All demonstrations are performed without real LPG flames  
User safety is prioritized over automation

Team & Contributions:
Saksham – Hardware integration & circuit assembly
Anshika – Sensor testing & embedded logic support
Siddharth – System architecture, flowcharts & documentation
Sunidhi – Use-case analysis, safety validation & demo presentation

Conclusion:

This project addresses a real-world household safety problem using IoT and embedded systems.
By combining early detection, automated response, and clear system logic, the solution aims to reduce gas-related accidents in an efficient and scalable way.
