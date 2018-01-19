# InfraredSensors
Using infrared sensors in collaboration with group members for robotic vacuum

### Table of Contents
1. [Introduction] (#introduction)
2. [Infrared Sensor Budget] (#IRBudget)
3. [Time Commitment] (#IRTime)
4. [Mechanical Assemly] (#IRMech)
5. [PCB Soldering] (#IRPCB)
6. [Power Up] (#IRPower)
7. [Unit Testing] (#IRUnit)
8. [Production Testing] (#IRProduct)
9. [Reproducible] (#IRReproducible)

### Introduction to Infrared Sensors

For my chosen project it was the use of an infrared sensor(IR) in collaboration with my classmate Kyle Sy. 
The project will utilize my partners sensors a motor driver and ultrasonic to create a robotic vacuum.
The infrared sensor will be used in detection of objects that come to or near the robotic vacuum.

![System Diagram](https://github.com/arZone1/InfraredSensors/blob/master/Hand-Ins/sysdiag.jpg?raw=true)

### Budget Of Materials

The materials required for this project was:
  - Raspberry pi 3 kit ($99.99)
  - Infrared sensor detection module ($10.99)
  - Male to Female , Female to Female jumper wires ($14.99)
  - LED ($3.99)
All of these items are available to purchase through Amazon

### Time Commitment 
-The time needed to complete my part of the project was setting up the raspberry pi which took about 20-30 minutes.
- Doing a dry test run of the module and wiring it to a breadboard to ensure it works and powers on taking 45 minutes. 
-Creating the pyton code on the raspberry pi 30-45 minutes needed to run and test the code
Overall the needed time to complete this build should be around 2 hours.

### Mechanical Assembly 

The mechanical assembly is wiring the sensor onto the breadboard and using the GPIO header pins. My sensor only had 3 pins that needed to be connected the Vcc, Gnd and Out. 
The pyton code will read the data from:
- pin 2 for 5v Vcc,
-GPIO pin 9 for ground 
-pin 11 for GPIO 17. 
Also wiring a LED to the output and ground will light up upon detection. Below is the wiring before plugging it into power. Also shown is the LED lighting up.

![Assembly](https://github.com/arZone1/InfraredSensors/blob/master/Hand-Ins/pitest.jpg?raw=true)

### PCB Soldering 

There was no soldering required with my sensor due to it being able to be connected directly to the raspberry pi using female to female connectors. For testing purposes I had connected the sensor to the breadboard and using female to male connectors.

### Power Up

Powering up the raspberry pi the sensor will work without the code running due to the module being wired up directly to power and the output will be adjustable because the potentiometer being turned left or right. Running the code will allow for setting the output and getting detection where the LED will turn of on detection and left on when it is waiting for something to come in the way.

![PowerOn](https://github.com/arZone1/InfraredSensors/blob/master/Hand-Ins/piOn.jpg?raw=true)
### Unit Testing 
-	Checking if the IR is detecting anything in the way of the sensor if there is detection in front of the IR cause the LED to turn ON
-	Checking the IR if nothing is in the way of the IR cause the LED to stay OFF
-	Wiring the LED to the module positive to the anode and negative to the cathode of the LED
-	Testing the python code to read the data from the IR

### Production Testing 
Powering the raspberry pi the module should already be running due to it being wired directly to the Pi and detection will already be scanning.
Reproducible 
If a user wants to make a simple detection for an infrared obstacle voidance sensor they will be able to. Detection can be used to stop an operation such as a garage opener or closer. For example if the car is approaching the sensor will have detection and the door will not close on the person driving.
