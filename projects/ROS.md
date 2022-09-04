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
<img class="img-fluid" src="../img/ROS.png">

Robot Operating System (ROS) is a set of libraries and tools to help you build robot applications. ROS was installed onto a Raspberry Pi 4 and integrated with ArduPilot on a Kakute H7 flight controller to retreive onboard sensor data. 

ROS utilizes "nodes" which may publish data to a "topic". Other nodes may then subscribe to a topic to receive the data that was published to it. To communicate between ROS and the ArduPilot firmware, a MAVROS node was utilized. This allowed ArduPilot to send data to ROS and vice versa. Using the MAVROS node, I was then able to retrieve sensor data, specifically the Inertial Measurement Unit (IMU) data from the gyroscope, accelerometer, and magnetometers. IMUs are used to measure acceleration, angular velocity, and magnetic fields and can be used to determine motion, orientation, and heading of an object.  

<img class="img-fluid" src="../img/ardupilot.png"width=35% height=35%>

Using MAVROS, certain parameters and states of ArduPilot are able to be modified. One such parameters is the message data stream rate parameter. We are able to reduce the data stream rate of unnecessary messages, reducing the total bandwidth used. The vehicle may also be controlled autonomously by sending commands that mimic RC inputs and RC inputs may also be read and stored by ROS. In addition to mimicing RC inputs, waypoints may also be sent to the waypoint list for an autonomous flight. 

While i only have a few months of experience working with ROS integrated with ArduPilot, I have learned a lot and have come to appreceite how ROS can positively affect unmanned autonomous vehicles. I am eager to learn more about the ins and outs of ROS and maximize the potential that Robot Operating System can bring to the unmanned autnomous vehicle environment.
