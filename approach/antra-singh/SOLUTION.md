CAMPUS DELIVERY ROBOT PROJECT 
Features: 
1.	Movable in order to deliver items.
2.	Storage to store the delivery item. 
3.	Terrain Detection so that  it doesn’t falls from stairs, don’t go to mud, uneven land.
4.	Face Recognition to recognize the person to whom order is to be delivered.
5.	Obstacle Detection so that robot doesn’t collide. 
6.	Vehicle Detection so that robot do not get crushed by ongoing vehicles. 
7.	Collision Avoidance Once obstacle is detected robot must know how to avoid going to that path and figure out some alternative path.
8.	Emergency Alert If in danger robot must send emergency alert
9.	Power Supply
Challenges: 
1.	Microcontroller may not be able to  support heavy ML models used for Terrain Detection, Face Detection , Obstacle Detection, Vehicle Detection and Collision Avoidance. 
2.	Robot may not be able to cross Stairs and may collide.

SYSTEM DESIGN
1.	Microcontroller : ESP32 CAM
Reason : 
1) It supports live video streaming in low resolution which is needed to detect terrain  and for face detection. 
2) Supports light ML model which is needed so that robot can take decisions to avoid collision and when to send emergency alerts. 
3) Contains inbuilt Wifi and Bluetooth. 
4) Budget Friendly. 
2.   Movable : 
1) Body :  Wheels * 4 (Diameter of wheels = Diameter of Stairs)
2) Motor : DC Motor * 4
3)  Motor Driver (In order to control robot’s speed and movement) :  L298N / L293D * 1
3. Terrain Detection : Since ESP32 does not supports models like YOLO or OpenCV for terrain detection, one can use camera frame and TensorFlow Lite Micro to support light ML Models and another alternative to it is ESP32-CAM + IMU + Vision. MPU6050 IMU can be used to detection earthly vibrations like slope and bumps if present and with the help of ESP32-CAM we can input terrain. 
4. Face Recognition : ESP32  CAM has a built in Face recognition model in ESP32 Web cam server and for more accuracy one can use ESP-WHO, a framework for face detection and recognition written in C/C++. 
5. Obstacle Detection: Ultrasonic Sensor for range approx. 2cm to 4m. 
6. Vehicle Detection :  TinyML + object detection can be used.
7. Collision Avoidance: To avoid collision and take alternative path a ML model can be trained using Deep Q Network, Proximal Policy Optimization and DDPG algorithms and mapping can be used so that robot can make decision take alternative path.
8. Emergency Alert : Train Robot to Detect emergency using TensorFlow for detecting accident, Predict crash based movement using RNN, RL.
IMPLEMENTATION 

Phase 1: Design a robot virtually using Autodesk  Fusion 360, Blender and Tinkercard, a working model.
Phase 2 : Assemble the Mechanical and electronical part physically as per the virtual design. 
Phase 3 : Integrate ML Model and Programs to microcontroller.







