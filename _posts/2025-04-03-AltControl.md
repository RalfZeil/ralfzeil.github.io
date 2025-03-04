---
title: "Alt Control - Weather Dome"
date: 2023-09-27
author: "Ralf Zeilstra"
categories: [Projects, Alternative Control]
tags: [Unity, ESP-32, NDI, Dome Projection]
---

{% include embed/youtube.html id='dKd2wDL-zZU' %}

### Context
The project _Alt Ctrl_ is inspired by GDC's Alt Ctrl event. It focuses on creating alternative controllers for games.  
The duration of the project was a little less than two weeks.

### Design Choices
For this project, I made deliberate design choices that significantly influenced its development.  
Utilizing the dome was a pivotal decision. The dome is an installation at HKU with a "360 Dome" where you can project 1:1 images with four projectors on a half-spherical surface.  
The ability to dynamically rotate the sun 180 degrees around the world adds a captivating visual dimension.  
The controller design echoes this immersive experience, integrating a potentiometer that mirrors the sun's movement within the Unity scene.  
Additionally, I implemented a lightning weather effect as both a functional element and a proof-of-concept.

![Alt Control Thumbnail](./assets/images/AltCtrl/Hardware1.png)  
![Dome View of Unity](./assets/images/AltCtrl/DomeViewOfUnity.jpg)  

### How It Works
The program is rendered using Unity Engine on my laptop. A Unity plugin facilitates the transmission of live video over NDI (Network Device Interface) to the Dome PC.  
Input is tracked using an ESP-32 microcontroller, which captures data from a potentiometer and a button, transmitting it to the serial port.  
Within Unity, I used C# to interpret and integrate this data.

![Final Scene](./assets/images/AltCtrl/FinalScene.png)  

### Issues During the Project
The biggest hurdle was the inability to transmit images over NDI. Despite troubleshooting, the root cause remains unclear.  
Performance issues within the Unity scene also posed challenges. Transitioning from HDRP to URP helped, but the script reading the serial port struggled to keep up with the render loop, requiring threading for optimization.

![Dome Setup](./assets/images/AltCtrl/DomeSetup.png)  
![Hardware](./assets/images/AltCtrl/Hardware2.png)  

### Used Tools & Other Links
- [Unity Engine](https://unity.com)  
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/)  
- [Arduino IDE](https://www.arduino.cc/en/software)  
- [Arduino IDE ESP32 Library](https://github.com/espressif/arduino-esp32)  
- [KLAK NDI](https://github.com/keijiro/KlakNDI)  
- [Dome Tools](https://assetstore.unity.com/packages/vfx/shaders/fullscreen-camera-effects/dome-tools-62664)  
- [Nature Starter Kit](https://assetstore.unity.com/packages/3d/environments/nature-starter-kit-2-52977)  
- [Snowy Mountain](https://assetstore.unity.com/packages/3d/environments/high-quality-free-snowy-mountain-game-ready-233788)  
- [RPG VFX Bundle](https://assetstore.unity.com/packages/vfx/particles/spells/rpg-vfx-bundle-133704)  
