---
layout: project
type: project
image: img/ROS.png
title: "ROS"
date: 2022
published: true
labels:
  - ROS
summary: "Implemented Robot Operating System (ROS) with ArduPilot to Retrieve Sensor Data"
---

Robot Operating System (ROS) is a set of libraries and tools to help you build robot applications. ROS was installed onto a Raspberry Pi 4 and integrated with ArduPilot on a Kakute H7 flight controller to retreive onboard sensor data. 

ROS utilizes "nodes" which may publish data to a "topic". Other nodes may then subscribe to a topic to receive the data that was published to it. To communicate between ROS and the ArduPilot firmware, a MAVROS node was utilized. This allowed ArduPilot to send data to ROS and vice versa. Using the MAVROS node, I was then able to retrieve sensor data, specifically the Inertial Measurement Unit (IMU) data from the gyroscope, accelerometer, and magnetometers. IMUs are used to measure acceleration, angular velocity, and magnetic fields and can be used to determine motion, orientation, and heading of an object. 
