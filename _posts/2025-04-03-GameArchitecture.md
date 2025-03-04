---
title: "Game Architecture"
date: 2023-10-08
author: "Ralf Zeilstra, Max Bronstring"
categories: [Projects, Game Architecture]
tags: [Unity, C#, Game Development, Modular Design]
---

{% include embed/youtube.html id='6GPcstzQzRE' %}

### Context
This is a small prototype made for an exercise for _Game Architecture_.  
The subject focuses on developing modular and clean code, systems, and applying code patterns.

### The Project
Together with another game programmer/developer, I created this simple prototype featuring a crafting, inventory, and building system working together.  
My part of the project was creating the building system.  
There were a few limitations set on us to increase the need for more careful planning.  
We were only allowed to inherit from Unity's `MonoBehaviour` once.

![Behaviour Flow Diagram](./assets/images/GameArchitecture/BuildingDiagram.png)

### Tech/Systems Used
For this project, we used **Unity** and **C#** to create this prototype.

### Used Tools & Other Links
- [Unity Engine](https://unity.com)
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/)
- [draw.io](https://app.diagrams.net/)
