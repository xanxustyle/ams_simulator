# `AMS Simulator`: ROS/Gazebo simulations of Autonomous Marine System (AMS)

[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://github.com/xanxustyle/ams_simulator/blob/main/LICENSE)

The **Autonomous Marine System Simulator** is a [ROS 1](http://wiki.ros.org/)- and [Gazebo](http://gazebosim.org/)-based simulation environment for fast-prototyping and evaluation of marine robotic systems. The packages are built upon the [UUV Simulator](https://github.com/uuvsimulator/uuv_simulator).

# Features

> **ROS/Gazebo Plugins**
  
- Implementation of Fossen's equations of motion for underwater vehicles
- Thruster modules with implementations for thruster's angular velocity to output thrust force based on [`Yoerger el al., 1990`](http://dx.doi.org/10.1109/48.107145) and [`Bessa et al., 2006`](http://www.abcm.org.br/symposium-series/SSM_Vol2/Section_IX_Submarine_Robotics/SSM2_IX_01.pdf)
- Lift and drag plugin for simulation of fins
- Simulation of 3D current velocity models (constant or based on first-order Gauss-Markov processes)
- Sensor plugins

> **Controllers**

- [`casadi`](https://web.casadi.org/)-based effort allocation algorithm 
- Geometric tracking PD controller
- Non-model-based sliding mode controller ([`García-Valdovinos el al., 2014`](https://journals.sagepub.com/doi/full/10.5772/56810) and [`Salgado-Jiménez et al., 2011`](http://cdn.intechopen.com/pdfs/15221.pdf))
- Teleoperation nodes for AUVs and ROVs

> **Gazebo World Models**

- Ocean wave shaders for wave animation
- Stratified transient ocean current model
- Scenarios of coral reef environments

> **Vehicle Models**

- [`RTSys NemoSens`](https://rtsys.eu/nemosens-micro-auv)
  
# Installation

This package requires ROS Noetic and Gazebo 11 on Ubuntu 20.04 Focal Fossa (64-bit).

- `Noetic Ninjemys` (See [installation instructions for ROS Noetic](https://wiki.ros.org/noetic/Installation/Ubuntu))
- `Gazebo 11` (See [installation instructions for Gazebo 11](https://classic.gazebosim.org/tutorials?cat=install&tut=install_ubuntu&ver=11.0))

# Purpose of the project

This software is a research prototype, developed for the Autonomous Sensor Future Science Platform (AS FSP) Project.

The software is not ready for production use. However, the license conditions of the applicable Open Source licenses allow you to adapt the software to your needs. Before using it in a safety relevant setting, make sure that the software fulfills your requirements and adjust it according to any applicable safety standards (e.g. ISO 26262).

# License

AMS Simulator is open-sourced under the Apache-2.0 license. See the
[LICENSE](https://github.com/xanxustyle/ams_simulator/blob/main/LICENSE) file for details.

For a list of other open source components included in UUV Simulator, see the
file [3rd-party-licenses.txt](https://github.com/uuvsimulator/uuv_simulator/blob/master/3rd-party-licenses.txt).

# Releases

[![ROS Noetic](https://img.shields.io/badge/ROS%20Distro-noetic-brightgreen.svg)](http://repositories.ros.org/status_page/ros_melodic_default.html?q=uuv_simulator)
