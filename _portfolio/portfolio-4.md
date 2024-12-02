---
title: "Pneumatic Muscle Amplifier Exoskeleton"
excerpt: "![alt text]([https://github.com/jordanirgang/JIportfolio/blob/master/images/snapglove.jpg?raw=true](https://github.com/jordanirgang/JIportfolio/blob/master/images/icra-jordan-irgang.png?raw=true))<br/><br/>An ongoing personal research project I am designing to help my friend in a wheelchair by making an amplifier exoskeleton that if he moves a muscle, this will continue the motion for him."
collection: portfolio
youtubeId: c8Sa4B728Yo
---

<br>
## Project Use Case 
This project was created for the MakeMit 2022 hackathon where the team passed the initial pitch round and received $500 funding. I was personally invested in this project as I  believed that this experiment would assist my longtime friend in a wheelchair to use his muscles again and regain autonomy in his life. Before this hackathon I was learning how to build Pneumatic Air Muscles (PAMs).

## Project Functionality
An EEG MYOWear muscle sensor was placed on the arm and would send commands to a Raspberry PI if it detected nerve bioelectrical activity. It would then open and control pneumatic solenoids controlling the robber air muscles connected to an exoskeleton.

## My Role
- Designed and assembled PAM.
- Modeled Diagrams for software and P&ID piping drawings.
- Designed and printed Exoskeleton.
- Coded Python software for interfacing MYO EEG sensor to Solenoids, and also interfacing with an android app over TCP sockets.

## Next Steps
- As this is an important project to me I been continuously researching and developing ideas:  
    - Build PID controls for precise muscle movement 
    - Research control math and required state space models that could approximately model the dynamics of inflating the muscle.
    - Reprint the exoskeleton for increased comfort, usability, and ergonomics.
    - Test with my friend.
