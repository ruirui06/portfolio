## About me
I am a Junior Engineer who is passionate about Robotics and Mechatronics. 

### Techincal Skills:
- Mechanical Design & CAD: SolidWorks, AutoCAD, Fusion 360, Mechanical Assemblies, 3D Modeling, Engineering Drawings
- Analysis & Simulation: ANSYS (Fluent, Icepak)
- Prototyping & Testing: FDM/SLA 3D Printing, Laser Cutting, Soldering, Mechanical Assembly, Bench Testing
- Programming & Controls: C++, Python, MATLAB, Arduino
- Hardware Platforms: Raspberry Pi, ESP32, Sensors

## Education
Master of Science in Mechanical Engineering | San Jose State University at San Jose,CA,USA (_September 2023 - May 2025_)
Bachelor of Engineering in Mechanical | Carleton University at Ottawa,ON,Canda (_September 2018 - April 2022_)


## Projects
### Design and Implementation of a Feedback Controller for a Bio-Inspired Hand Exoskeleton

[Publication](https://doi.org/10.1115/IMECE2025-166983)

A feedback-controlled, synergy-based hand exoskeleton was developed for post-stroke rehabilitation. A soft, sensorized glove with potentiometers detects hand movements, processed by an **Arduino** to control linear servo actuators via TTL communication. Encoders enable precise, real-time replication of finger gestures. Using a synergy model, two actuators drive all five fingers, resulting in a lightweight (423 g), low-cost (~$440), fully 3D-printable design. Tests showed consistent 0.3 s response times across speeds, confirming suitability for real-time rehabilitation. Design updates including an improved actuator casing, enhanced straps, and a refined synergy mechanism improved comfort and adaptability.

#### System Architecture

- 2 linear servo actuators control five fingers via synergy grouping.
- Fully 3D-printed mechanical structure (PLA) with redesigned actuator mounts.
- Custom mechanical coupling for improved force transmission.
- Arduino-based controller with UART to TTL communication.

![SYSTEM SCHEMATIC](/assets/img/schematic.png)

#### Control & Embedded System

- MightyZap 12 Lf-17PT-53 linear actuators with built-in encoders.
- Real-time potentiometer input mapped to actuator API position values.
- Close-loop position feedback via half-duplex TTL communication.
- Dualk-actuator synchronization validated under variable speed condition.

<p align = "center"><img src="/assets/img/realsetup.png" width="50%"/>

#### Performance Results

- Consistents 0.3 s response time across 100%, 50%, and 25% speed settings.
- Stable dual-actuator communication without significant tracking error.
- Demonstrated real-time trajectory replication suitable for rehabilitation use.
- Latency primarily attributed to UART communcation overhead.
