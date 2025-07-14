# Automatic-Light-System
Project Overview:
This project presents a simple yet effective automatic lighting system using an Arduino microcontroller, an ultrasonic sensor (HC-SR04), an LDR (Light Dependent Resistor), and an LED. The system is designed to automatically control a light source based on ambient brightness and the proximity of an object.

It provides an energy-efficient solution for smart lighting — ideal for entryways, cupboards, or any environment where hands-free automatic lighting is beneficial.

Key Features
 Object Detection: Uses an HC-SR04 ultrasonic sensor to detect any object within 20 cm.

 Ambient Light Sensing: Monitors ambient light levels via an LDR.

 Auto Lighting: Turns ON the LED when it’s dark or when an object is nearby.

 Simple Logic: LED stays OFF when the surroundings are bright and no object is close.

Components Used
Component	Description
Arduino Board	Uno, Nano, or any compatible
HC-SR04 Ultrasonic Sensor	For proximity detection
LDR	For detecting ambient light
10K Resistor	Pull-down resistor for LDR
LED	Acts as the light source
Jumper Wires	For connections
Breadboard	For prototyping

 Circuit Connections
Component	Arduino Pin
HC-SR04 Trig	D2
HC-SR04 Echo	D3
LDR (via voltage divider)	A0 or D4
LED	D8

 Note: Connect the LDR in a voltage divider configuration with a 10K resistor between VCC and GND, with the middle point connected to A0 or D4.

 Working Principle
Light Check: The LDR measures ambient brightness. If the light level is below a threshold (i.e., it’s dark), it flags the LED to turn ON.

Distance Check: Simultaneously, the ultrasonic sensor detects any object within 20 cm of range.

LED Control:

If either low light OR object detection condition is true → LED turns ON.

If both conditions are false → LED remains OFF.

 How to Use
Build the circuit on a breadboard as per the connection table.

Upload the Arduino sketch using the Arduino IDE.

Power the Arduino via USB or external source.

Observe the LED turning ON in dark or when an object comes near.

 Circuit Diagram
For a clear visual reference, please refer to the provided file:
circuit.svg

