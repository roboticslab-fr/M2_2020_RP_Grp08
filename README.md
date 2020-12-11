<h1 align="center">ROS_Turtlebot3_Navigation</h1>

## Technical Documentation


<p align="center">
  <p align = "center">
     <img  src = "assets/cover/kinetic.png" width=400 >
     <img  src = "assets/cover/t3_robot.png" width=400 height=330>
    
  </p>
</p>

## Table of contents

- [Introduction](#introduction)
- [Objectives](#objectives)
- [Methodology](#methodology)
- [Implementation](#implementation)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction

Robotics is one of the upcoming technologies that can change the world. With software, we can expand a robot's capabilities and by that, we can gives them life. If a robot exists, its capabilities such as control, sensing, and intelligence are realized using software. However, robotics software involves a combination of related technologies, such as computer vision, artificial intelligence, and control theory. Hence, developing software for a robot is not a simple task. It may require expertise in many fields. In order to help software developers create robot applications, one of the more popular robotics software frameworks that has been created is Robot Operating System (ROS).

There are many reasons why ROS is popular in robotics software development. One of them is its modular design. ROS was designed to be as distributed and modular as possible. Different tasks can be developed separately, giving developers choices: whether using completed parts from others or implementing by themselves. Moreover, it also provides hardware abstraction. An extensive knowledge of hardware is not required. A robot can be moved without much knowledge of specifiation of the robot or background mathematical in kinetics and dynamics. Hence, we can save our time and effort in development process. 

Within the scope of this project, we develop our robotics software using the platform TheConstruct. It is an online platform featuring Ubuntu as its operating system, combining with ROS kinetic and Gazebo as real world simulator, etc. The robot model is Turtlebot 3 Burger. There are 4 tasks we need to achieve via this project. They will be explained in details in the next section.

## Objectives

The goal of this project is to:

- Create a script to move the robot around with simple /cmd_vel publishing.
- Create the mapping launches, and map the whole environment.
- Create a move base system which allows publishing the goal to **move_base** and avoiding obstacles while reaching that goal. 
- Create a program that allows the robot to navigate within the environment following a set of waypoints.


## Methodology

#### What is ROS?

ROS (Robot operating system) is a BSD-licensed system which allows controlling robotic components from a PC. ROS system consists of independent nodes that can communicate with each other through publish/subscribe messaging model. 

#### General concepts

- ROS Master <br></br>
ROS Master allows nodes in the system to communicate to each other through messages. It can be considered as a lookup table where all information related to nodes can be found. Therefore, it can help different nodes to locate each other and to start sending the messages.

<p align="center">
  <p align = "center">
     <img  src = "assets/ros_master.png">
  </p>
</p>


- ROS Node <br></br>
ROS node, according to ROS wiki, is basically a process that performs computation. It can be seen as an executable program running inside our application. 
The first advantage that ROS node brings to our application is reduction of code complexity. The application is much easier to scale when we divide it correctly into different packages and nodes. Secondly, it provides a great fault tolerance. Nodes communicate through ROS, they are not directly linked to each other. Therefore, when one node crashes, the other nodes still work. And it is a good feature for debugging. Thirdly, different nodes that are written in different language like Python, C++ etc can still communicate to each other without any problem. Undoubtedly, this is the best feature since we can increase the execution speed of certain nodes by writing them in C++ instead of Python for example.

- ROS Topics <br></br>
ROS topic acts like a middleman who is responsible to transmit the data between nodes so that they can communicate. A node that wants some information for other node, must subscribe to the topic that the other node published to. 

- ROS Messages <br></br>
The name says it all. This is the data structure that nodes publish to the topic in order to communicate with other nodes. 

- ROS Services <br></br>

- ROS Action
aksdjakjsdakjsdkajsd
- ROS Packages
kasjkjaksdjakds
- ROS Basic Commands
aksdkajsdkajskdjakjsd


## Implementation

## Conclusion

## References
