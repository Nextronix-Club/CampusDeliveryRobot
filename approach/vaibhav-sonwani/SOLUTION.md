# Vaibhav Sonwani - CampusDeliveryRobot Solution

## Your Task
Provide your approach and solution perspective for building the CampusDeliveryRobot project.

## Instructions
1. Explain how you would approach this campus delivery robot project
2. What technologies would you choose?
3. What challenges do you foresee?
4. How would you design the overall system?
5. What would be your step-by-step implementation plan?

## Project Context
- Campus delivery robot using ESP32 CAM
- Students/staff can order items for delivery
- Robot navigates autonomously using basic commands (left, right, forward, back)
- Need web/app interface for users
- Must handle obstacles and errors

---
**Write your complete solution approach below:**
## Solution by vaibhav sonwani

### My Approach
*LiDAR + ROS2 Navigation* — Full ROS2-based stack with 2D LiDAR for mapping and robust navigation. Focus on safety, geofencing, and reactive planning (DWB/TEB).

### Key Technologies
- Raspberry Pi 4 / Jetson Nano  
- 2D LiDAR (RPLIDAR / Hokuyo)  
- ROS2 + Nav2 (global planner, DWB/TEB/SmacPlanner)  
- For Backend - MQTT/WebSocket 
- For Frontend - React/React Native UI

### Main Challenges Identified
- Higher cost and integration complexity.  
- To ensure reliability, the mechanical and electrical design must be robust.  
- Need thorough testing around humans and traffic because Campus environment is chaotic.
- Outdoor lighting ruins vision.

### Implementation Steps
1. Integrate LiDAR and build a reliable chassis with encoders.  
2. Install ROS2, map campus with SLAM, add AMCL localization.  
3. Configure global and local planners, tune parameters in field tests.  
4. Implement backend, safety modules, and OTP/QR delivery workflow.

### Additional Notes
This is pretty much the "do it right" path to take. You end up putting in more effort right from the start. But the performance holds up way better when you use it out in the real world.