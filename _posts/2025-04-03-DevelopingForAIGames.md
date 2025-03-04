---
title: "Developing for AI Games"
date: 2023-12-08
author: "Ralf Zeilstra"
categories: [Projects, AI, Game Development]
tags: [Unity, C#, AI, Boids, A* Pathfinding, Behaviour Trees]
---

### Context
This is a project made for the subject _Developing for AI Games_.  
In this subject, we had to create/solve three different Game AI challenges:  
1. Create a Boids simulation.  
2. Calculate a path in a maze using the A* algorithm.  
3. Create a behaviour tree for game characters using only code.

---

### Boids
This Boids simulation uses the three basic rules of Boids: alignment, cohesion, and separation.  
The player can change the settings of the Boids. For this specific project, I added a random modifier to make the Boids look more like flying or clawing bugs.

{% include embed/youtube.html id='mLs2t1O_lZk' %}

---

### A* Pathfinding
This exercise was about creating an A* pathfinding algorithm.  
A maze is generated, and the player can click on the maze to set a start and end point.  
The algorithm calculates the shortest path between the two points.  
The base project was provided by my teacher, and I implemented the A* algorithm.

---

### Behaviour System
The behaviour tree task involved creating a behaviour tree for game characters.  
The behaviour tree had to be created in code only and be usable in a game engine like Unity.

![Behaviour Tree Class Diagram](./assets/images/DevelopingForAIGames/ClassDiagram.png)  
![Behaviour Flow Diagram](./assets/images/DevelopingForAIGames/FlowDiagram.png)

{% include embed/youtube.html id='MMBjaLIBXbI' %}

---

### Used Tools & Other Links
- [Unity Engine](https://unity.com)  
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/)  
- [draw.io](https://app.diagrams.net/)  
- [Github Repository for Boids](https://github.com/RalfZeil/UnityBoids)  
- [Github Repository for A* Pathfinding](https://github.com/RalfZeil/KMOD3_Astar)  
- [Github Repository for Behaviour Tree](https://github.com/RalfZeil/BehaviourTreeExercise)  
