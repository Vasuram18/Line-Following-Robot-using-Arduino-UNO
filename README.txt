Line Following Robot Using Arduino Uno
Overview
This project involves the creation of a line-following robot using an Arduino Uno. The robot is designed to follow a black line on a white surface using infrared sensors. Additionally, it includes an ultrasonic sensor for obstacle detection, which stops the robot if an object is detected within a certain distance.

Features
Line Following: The robot uses two infrared sensors to detect the black line and adjust its direction accordingly.
Obstacle Detection: An ultrasonic sensor is used to measure the distance to obstacles in front of the robot, stopping the robot if an obstacle is too close.
DC Motor Control: The robot uses four DC motors controlled by the AFMotor library to drive and steer.
Components
Arduino Uno: The main microcontroller board for processing inputs and controlling outputs.
AFMotor Shield: A motor driver shield for controlling the DC motors.
DC Motors: Four motors to drive the robot.
Infrared Sensors: Two sensors for detecting the line.
Ultrasonic Sensor: Used for obstacle detection.
Miscellaneous: Breadboard, jumper wires, and power supply.
Installation
AFMotor Library: You need to install the AFMotor library before uploading the code.
Go to Sketch > Include Library > Add .ZIP Library and select the AFMotor ZIP file.
Code Explanation
The code initializes the sensors and motors, then enters a loop where it constantly checks the sensor inputs and adjusts the motor speeds to follow the line. The ultrasonic sensor measures the distance to any obstacles, stopping the motors if an obstacle is detected within 5 cm.

Circuit Diagram
Connect the infrared sensors to analog pins A4 and A5.
Connect the ultrasonic sensor's trig pin to A0 and echo pin to A1.
Connect the DC motors to the motor shield attached to the Arduino Uno.
Usage
Assemble the circuit as per the circuit diagram.
Install the AFMotor library in the Arduino IDE.
Upload the code to the Arduino Uno.
Place the robot on a track with a black line on a white surface and observe its movement.
Future Enhancements
Add more sensors for improved line detection.
Implement a more advanced algorithm for smoother turns.
Enhance obstacle detection to navigate around obstacles instead of stopping.
Acknowledgments
This project uses the AFMotor library for motor control.
The idea for a line-following robot was inspired by various online tutorials and resources.
License
This project is open-source and available under the MIT License.