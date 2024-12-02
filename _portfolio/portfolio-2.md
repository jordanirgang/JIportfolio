---
title: "Pixie Rover: PPE Detecting Hospital Robot"
excerpt: "![alt text](https://github.com/jordanirgang/JIportfolio/blob/master/images/gallery.jpg?raw=true)<br/><br/>A personal protection equipment(PPE) detecting robot designed to open and close IoT locks for safety protocol compliance."
collection: portfolio
youtubeId: I13JGnt3HKc
---

{% include youtubePlayer.html id=page.youtubeId %}
<br>
## Project Use Case 
In the medical world, protocol execution is extremely crucial to be followed and therefore this project hopes to utilize AI into a friendly looking robot to ensure compliance. This project was completed within 24 hours at a hackathon (including the CAD design and 3d printing).
![](https://github.com/jordanirgang/JIportfolio/blob/master/images/gallery2.jpg?raw=true)

## Project Functionality
TThe robot uses a Raspberry PI to record footage and upload the videos to an AI platform built for generating stories and summarizing footage, based on yes or no queries the robot will nod or shake its head to determine if the person is wearing PPE. The robot runs an onboard flask server with an HTML page for interface and API publish/receive events and can publish TCP commands to an ESP32 controlled electro lock. 
![](https://github.com/jordanirgang/JIportfolio/blob/master/images/gallery3.jpg?raw=true)

## My Role
I designed UML and timing diagrams for the main full stack programmer. I designed the robot and 3d printed each part in the same 24 hour time frame while building parts with correct tolerances for interfacing with COTS hole patterns for motors. Solved merge conflicts and programmed python based I2C interface with servo motor drivers.
![](https://github.com/jordanirgang/JIportfolio/blob/master/images/gallery1.jpg?raw=true)

## Next Steps
The webpage UI can have more complicated yes/no questions.
The robot was 3d printed as an open frame to expedite development and would be designed with an external skin.
The robot can be given wheel functionality for patrolling use cases.
