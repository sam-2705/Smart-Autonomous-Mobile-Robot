# Smart-Autonomous-Mobile-Robot
An Autonomous Mobile Robot (AMR) developed for Smart Factory Automation using Raspberry Pi, Arduino, OpenCV and Computer Vision.

Team ONIX
2nd Prize Winner  | ROBOAUTO-2026 Hackathon
Organized by IEEE Robotics Club, VJIT

About
The Smart Autonomous Mobile Robot (AMR) is an intelligent robotic system developed for ROBOAUTO-2026 under Theme 4 – Smart Automation. The robot is designed to simulate real-world smart factory operations by autonomously navigating through industrial environments, detecting obstacles, making adaptive decisions, and performing autonomous payload dumping.
The system combines Computer Vision, Embedded Systems, and Sensor Fusion to create a reliable autonomous mobile robot capable of completing industrial logistics tasks with minimal human intervention.

Problem Statement
Theme 4 – Smart Automation
Design and develop an intelligent Autonomous Mobile Robot (AMR) capable of integrating Smart Factory Automation, Adaptive Decision-Making, Autonomous Logistics, and Real-Time Industrial Process Management.
The robot should be capable of performing autonomous navigation, intelligent obstacle avoidance, and industrial material handling while adapting to dynamic environments.

Objectives:-
The primary objective of this project was to design and develop an intelligent Autonomous Mobile Robot capable of:
Autonomous navigation using Computer Vision
Adaptive decision-making in dynamic environments
Real-time obstacle detection and avoidance
Autonomous payload dumping at the designated destination
Reliable communication between Raspberry Pi and Arduino
Simulating smart factory logistics and automation

Competition Missions

Mission 1 – Autonomous Line Following
Develop an autonomous robot capable of navigating along the designated path using computer vision.
Our Solution:-
USB Webcam continuously captured live video.
Raspberry Pi processed camera frames using OpenCV.
The robot identified the navigation path and generated movement commands.
Arduino controlled the motors accordingly.

Mission 2 – Autonomous Payload Dumping
The robot had to reach the destination and autonomously dump the payload.
Our Solution:-
Robot continued autonomous navigation.
Destination marker was detected using HSV color detection.
Raspberry Pi instructed Arduino to stop.
Servo motor tilted the payload tray and completed the dumping operation.

Mission 3 – Intelligent Obstacle Avoidance
The robot had to identify obstacles, determine an alternate path, and reach the destination within minimum time.
Our Solution:-
Ultrasonic sensor continuously monitored obstacles.
Raspberry Pi and Arduino communicated in real time.
A Smart Scan algorithm was implemented.
Obstacle Detected
⬇
Reverse
⬇
Scan Left
⬇
Check Path
⬇
Scan Right
⬇
Check Path
⬇
Perform U-turn if required
⬇
Continue towards destination
This enabled adaptive decision-making while maintaining autonomous navigation.

Hardware Components:-
Raspberry Pi	
Arduino Uno	
USB Webcam 
L298N Motor Driver	
HC-SR04 Ultrasonic Sensor	
Servo Motor	
I2C LCD Display	
DC BO Motors	
Robot Chassis	
Wheels	
12V Battery	
Buck Converter

Software & Technologies:-
Python
Arduino IDE
OpenCV
NumPy
PySerial
Embedded C
Raspberry Pi OS

How It Works:-
The robot follows a layered architecture.

Raspberry Pi
Captures live video from the USB webcam
Performs Computer Vision using OpenCV
Processes Region of Interest (ROI)
Uses HSV color segmentation for object detection
Makes navigation decisions
Sends movement commands to Arduino

Arduino Uno
Controls DC motors
Controls servo motor
Reads ultrasonic sensor
Displays robot status on LCD
Performs emergency braking when obstacles are detected

Sensor Fusion
The robot combines data from:
Camera (vision)
Ultrasonic Sensor (distance)
This improves navigation accuracy and safety.

Results:-
Won Second Prize at ROBOAUTO-2026
Successfully completed Mission 1 – Autonomous Line Following
Successfully completed Mission 2 – Autonomous Payload Dumping
Successfully completed Mission 3 – Intelligent Obstacle Avoidance
Demonstrated adaptive decision-making using Computer Vision and Sensor Fusion
Achieved reliable communication between Raspberry Pi and Arduino

Team ONIX:-
Srivas Kashyap
Shashank Kondapalli
Sameena Shaik
Roopa Oruganti
Y. Karthik

Acknowledgements:-
We sincerely thank the IEEE Robotics Club, VJIT, for organizing ROBOAUTO-2026 and providing an excellent platform to innovate, collaborate, and apply engineering concepts to solve real-world automation challenges.
We also thank our mentors, faculty members, volunteers, and teammates for their continuous guidance and support throughout the hackathon.
