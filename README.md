# Intragration-Project
INF1900 - Final Project: Autonomous Obstacle-Navigating Robot

Course: INF1900 - Initial Embedded System Project
Institution: Polytechnique Montréal

1. Project Objective

This project is the final integrator for the INF1900 course. The primary objective was to design, build, and program an autonomous robot capable of navigating a complex, unknown track filled with obstacles.

This project served as a synthesis of all concepts covered during the semester, including:

Low-level hardware interfacing with an AVR microcontroller.

C++ programming for embedded systems.

Object-Oriented Programming (OOP) principles and design patterns.

Sensor data acquisition and processing.

Real-time motor control and decision-making.

Collaborative development using Git.

2. Technical Overview

Hardware

Microcontroller: Atmel AVR (ATmega) series on a custom motherboard.

Sensors: Infrared (IR) distance sensors for obstacle detection and environment mapping.

Actuators: Two DC motors for propulsion and differential steering.

Software & Libraries

Language: C++

Libraries: AVRLibC for low-level peripheral and register manipulation.

Development: Code was developed following course-specific quality standards and compiled using avr-gcc.

Version Control: Git was used for all version control and team collaboration.

3. Software Design

A significant focus of the project was writing high-quality, modular, and reusable code. The project was built using an Object-Oriented (OOP) approach rather than a purely procedural one.

Key software components include:

SensorManager: A class dedicated to initializing, reading, and filtering data from the IR distance sensors.

MotorControl: An interface for controlling the robot's movement, managing PWM signals for speed, and handling direction (forward, backward, turns).

NavigationLogic: A high-level state machine that takes processed sensor data as input and makes real-time decisions about the robot's next action (e.g., MOVE_FORWARD, AVOID_OBSTACLE_LEFT, STOP).

Interrupts / Polling: An analysis was performed to determine the best strategy (interrupts vs. polling) for managing sensor data acquisition without blocking the main control loop.

4. Repository Structure

The code is organized as required by the course guidelines:

/
├── exec/        # Main application code containing the robot's logic and state machine
├── lib/        # Reusable libraries and hardware drivers (e.g., AVRLibC)
└── README.md   # This file


5. Acknowledgments

We would like to thank the entire INF1900 teaching staff for their guidance and support throughout this project, including Professor Jérôme Collin, the technical support staff, and our lab instructors.
