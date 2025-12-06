WiFi-Powered Robot — Final Project (Arduino UNO R4 WiFi)
By: Lucy Hennessy
📌 Overview

This project showcases a fully WiFi-controlled robot built using the Arduino UNO R4 WiFi, an ultrasonic sensor, and a custom web-based control interface. The robot accepts directional commands (Up, Down, Left, Right) from any web browser and incorporates obstacle detection for enhanced safety.
All movement, sensor logic, and UI styling were coded from scratch and tested across multiple iterations. 

Robotics Final Report

✨ Features

WiFi Remote Control via a browser-based interface

Four movement commands: Up, Down, Left, Right

Ultrasonic obstacle detection with automatic stopping

LED matrix alert that displays a circular warning symbol when objects are too close

Auto-resume logic when the obstacle is removed

Custom HTML/CSS interface styled with Kent State colors, hover states, and responsive design

Real-time serial feedback for debugging and monitoring system behavior

🛠 Hardware Used

Arduino UNO R4 WiFi

Ultrasonic Sensor (HC-SR04)

Dual Motor Driver

DC Motors + Wheels

LED Matrix

External Battery Pack

Breadboard + jumper wires

Wiring diagrams and photos of the assembled robot can be found in the report. 

Robotics Final Report

💻 Software & Code Structure

The robot runs Arduino C++ code that handles:

Movement Control

Functions for controlling each motor, stopping, resuming, and direction-based wheel speeds.

WiFi Server

A local web server allows browser-based button presses to send commands to the motors.

Sensor Logic

Reads distance continuously and enforces:

Stop when distance < 15 cm

Resume when distance > 20 cm

LED Matrix UI

Displays a circle when the robot stops for safety.

Web Interface

A responsive HTML page is served directly from the Arduino, featuring:

Large directional buttons

Hover animations

Click effects

A clean KSU-themed control panel

Full code is provided in the repository (and in the report). 

Robotics Final Report

🧪 Testing & Debugging Summary

Throughout development, we debugged several issues, including:

Motors spinning in the wrong direction → fixed by checking wiring and adjusting motor logic

WiFi connection failures → solved by resetting the port, IDE, and using a hotspot

Incorrect ultrasonic readings → traced back to swapped trig/echo wires

Robot not resuming movement → refined control logic to handle manual vs. automatic modes

This testing process helped us refine both wiring and code functionality. 

Robotics Final Report

📱 Web Control Page Design

The control page uses:

Game-style directional layout

Blue & gold Kent State theme

Responsive sizing for mobile/desktop

Simple, emoji-free buttons for compatibility with Arduino’s server

The goal was a clean, intuitive UI that works on any device. 

Robotics Final Report

📚 Project Reflection
Biggest Challenge

Getting the robot to intelligently stop and later resume movement after detecting obstacles.

Team Roles

One member focused primarily on wiring, hardware assembly, and TinkerCAD

The other focused on coding, WiFi server setup, HTML styling

What We Learned

Debugging requires patience, iteration, and checking both hardware and software step-by-step.

Future Improvements

Full autonomous navigation

More sensors for 360° detection

Adjustable speed (manual slider or autonomous speed control)

Real-World Applications

This system models real robotics found in delivery bots, warehouse machines, and smart home devices.
