---
title: "General Use PID Controller C++ Framework"
excerpt: "![alt text](https://github.com/jordanirgang/JIportfolio/blob/master/images/downloadcrop.png?raw=true)<br/><br/>In order to bring closed loop motor control costs down, this framework will read a potentiometer/encoder and a motor and apply PID controls. This is being built to support my future projects."
collection: portfolio
---

## Project Functionality
Generic C++ classes for handling motor control and sensor reading contain functionality logic for how the sensor in theory should work. The implementation is called through arduino based extended classes so extra functionality can be written for different hardware use cases. Unit testing is embedded into the system via PlatformIO’s incorporation of  Unity(an embedded systems single file c based unit test framework) where additional features are regression tested automatically.
Math and theoretical proof of concepts are written in Python Jupyter books, where the discrete system is simulated with SymPy, Numpy, and MatPlotlib.

![](https://github.com/jordanirgang/JIportfolio/blob/master/images/download.png?raw=true)

## My Role
- Designed UML and timing diagrams for the main full stack programmer.
- Designed the robot and 3d printed each part in the same 24 hour time frame while building parts with correct tolerances for interfacing with COTS hole patterns for motors.
- Solved merge conflicts and programmed python based I2C interface with servo motor drivers.

![](https://github.com/jordanirgang/JIportfolio/blob/master/images/thumbnail3.png?raw=true)

## Next Steps
- The webpage UI can have more complicated yes/no questions.
- The robot was 3d printed as an open frame to expedite development and would be designed with an external skin.
- The robot can be given wheel functionality for patrolling use cases.
