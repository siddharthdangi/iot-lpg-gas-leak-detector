#IoT-Based LPG Gas Leak Detection & Automatic Cut-Off System
Problem Statement:

In most Indian households, LPG cylinders are used for daily cooking. Gas leakage, faulty regulators, or accidentally leaving the stove ON can lead to serious accidents such as fire, explosions, or health hazards.
Existing safety methods mainly rely on human attention and local alarms, which may fail when users are not present at home.

Proposed Solution: 
We propose an IoT-based smart LPG gas safety system that continuously monitors gas levels near the stove or regulator area and automatically reacts in case of danger.

The system:

1) Detects LPG gas leakage using a gas sensor

2) Provides instant local alerts (buzzer & LED)

3) Uses a controller-based decision logic

4) Simulates automatic gas cut-off

5) Is designed as a non-invasive external add-on, without modifying government-issued LPG regulators

Hardware Components Used:
1) ESP32 Development Board

2) MQ-5 Gas Sensor

3) Active Buzzer 

4) LED with resistor

5) Breadboard

6) Jumper wires

7) USB power supply

8) (Servo / solenoid valve planned for next round)

System Architecture & Working:

1) The gas sensor continuously measures gas concentration.

2) The ESP32 reads the analog sensor value.

3) The value is compared with a predefined safety threshold.

4) If gas concentration is below threshold:

5) System remains in monitoring state.

If gas concentration exceeds threshold:

1) Buzzer and LED are activated

2) Gas cut-off logic is triggered (simulated)

3) Alert message is generated

Prototype Status (Round-1 Submission):

1) Gas detection using MQ sensor is functional

2) ESP32 successfully processes sensor data

3) Buzzer and LED alert system works correctly

4) Gas cut-off is logically implemented (simulated)

5) Serial Monitor used for real-time monitoring and alerts

6)This prototype demonstrates the core functionality and feasibility of the system.

Planned Enhancements (Round-2 Scope):

1) In the next stage, the system will be enhanced with:

2) Physical gas cut-off using servo motor or solenoid valve

3) Compact clip-on enclosure compatible with LPG regulators

4) Mobile notification using IoT platform (Blynk/Firebase)

5) Improved false-alarm filtering

6) Battery backup for power failure

7) Multiple sensor placement for better coverage

Safety & Ethics Consideration:
1) The system is designed as an external safety attachment

2) It does not replace or modify government-issued LPG regulators  

3) All demonstrations are performed without real LPG flames  

4) User safety is prioritized over automation

Team & Contributions:
1) Saksham – Hardware integration & circuit assembly

2) Anshika – Sensor testing & embedded logic support

3) Siddharth – System architecture, flowcharts & documentation

4) Sunidhi – Use-case analysis, safety validation & demo presentation

Conclusion:

This project addresses a real-world household safety problem using IoT and embedded systems.
By combining early detection, automated response, and clear system logic, the solution aims to reduce gas-related accidents in an efficient and scalable way.
