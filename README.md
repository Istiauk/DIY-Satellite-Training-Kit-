# DIY-Satellite-Training-Kit-
Low-Cost DIY Satellite Training Kit (1U CubeSat)

A do-it-yourself satellite training kit built from locally available components in Bangladesh, so that students and electronics hobbyists can get hands-on experience building a basic 1U CubeSat. The kit covers power, on-board computing, communication, a camera payload, a ground base station, and a backplane that ties everything together.

Course project: EEE/ECE 383, Fall 2023 (report dated 31 December 2023), BRAC University.

<p align="center"> <img src="images/final-assembly.jpg" alt="Final assembly of all subsystems" width="520"> <br><em>Final design: all subsystems integrated on the backplane</em> </p>
Motivation

Bangladesh has strong STEM talent in electrical and electronic engineering and computer science, but little participation in space technology. The main reasons are scarce educational resources and the high cost of components. This project aims to lower that barrier with a simple, affordable kit that teaches electronics, communication engineering, and programming through hands-on building.

Objectives
Develop an affordable DIY satellite training kit.
Use components that are widely available in local markets.
Keep the design approachable for college and university students.
Let students and hobbyists build their own satellite, communication, and space-related projects.
Build interest and participation in space technology in Bangladesh.
Main mission
Establish a link with the ground station.
Send sensor telemetry to the ground station.
Use the satellite to rebroadcast (digipeat) transmitted packets over a wider area.
Capture and transmit video from an on-board camera.
System Overview
Subsystem	Role	Key components
EPS (Electrical Power System)	Battery pack, solar charging, voltage regulation, MOSFET power switching	4× 18650 Li-ion (3.7 V, 2600 mAh), Mini360 buck converters, IRF9540 (P-ch) / IRF540 (N-ch) MOSFETs, Schottky diodes
OBC (On-Board Computer)	Collects telemetry, receives ground commands, switches modules on/off	Arduino Nano, MPU6050 IMU, BMP180 barometer, LM35 temperature sensor, SX1278 LoRa, L7805 regulator
Payload & COM	Camera video link and LoRa data link	1000TVL FPV camera, TS5828L 5.8 GHz 600 mW video transmitter, LoRa E32 (1 W), Arduino Nano
Base Station	Ground-side receiver and user interface	2× Arduino Nano, 2× LoRa SX1278, SKYDROID 5.8 GHz UVC receiver, laptop UI
Backplane	Mechanical and electrical interconnect between subsystems	3× 2×20 female headers (2.54 mm pitch), 90 × 90 mm two-layer PCB
