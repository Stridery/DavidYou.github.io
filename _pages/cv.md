---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Research Projects
======
Design and Optimization of Ray Tracing System (Independent Project)                              7/2022-10/2022<br>
Supervisor: Prof. James F. O'Brien, University of California, Berkeley<br>
▪	Designed and implemented a fundamental light tracing system based on C++ in Visual Studio<br>
▪	Realized the functions of reading text information about the position, material, and direction of objects, light sources, and cameras in the scene, rendered and output complete scene images, etc.<br>
▪	Designed bounding box and octree algorithm to simplify the detection algorithm of light and object intersection, achieving at least 50% rendering acceleration<br>

Tank Battle Game Design (Group Project: 3 Persons)                                               5/2022-6/2022<br>
Supervisor: Prof. Zheng He, Wuhan University<br>
▪	Designed a 2.5 D duel game based on the Unity 3D platform using C#<br>
▪	Implemented basic operational logic of the tank, such as moving, firing (generating shells and assigning initial speed), deducting health points after detecting the collision between shells and the tank, and dying after the tanks’ health point reaches 0, realized the generation of random items and collision interaction with tanks, set several drop points on the map, generated and refreshed a scene every five seconds on the map, changed tanks attributes after the collision, etc.<br>

Course Project for Computer Organization and Design (Independent Project)                          3/2022-5/2022<br>
Supervisor: Prof. Yili Gong, Wuhan University<br>
▪	Used Verilog to implement CPU, including the implementation of ALU module, storage module, CPU Control module, etc., enabled the project to simulate the majority of primary instructions under the real RISC-V architecture, including calculation instruction, various load/store instructions, jump instructions, etc.<br>
▪	Implemented a pipeline structure and a hazard detection and processing model, used the Vivado tool to debug the hardware circuit and successfully run the program on the FPGA circuit board to calculate the Fibonacci sequence, etc.<br>


Internships
======
PICC Property and Casualty Company Ltd., Tech Operation Dept., System Development Intern, Chengdu   6/2023-8/2023<br>
▪	Participated in the backend development of the ‘Cloud Ladder’ process management platform and completed three iterative development tasks for the low-code platform  <br>
▪	Designed and realized functions such as customizing query, automatic task scheduling strategy configuration, configuration implementation of multi-table addition, deletion, modification, and query function, and the construction of a large model to generate prompt words based on database metadata via SQL<br>
▪	Wrote Cucumber test scripts, ensured demands implementation, and helped with the new version of ‘Cloud Ladder’ go live<br>

Beijing E-TECHSTAR Co., Ltd., Electrical Power Department, Software Engineer Intern, Beijing          7/2021-9/2021<br>
▪	Mainly engaged in frontend development tasks and studied Vue and uni-app<br>
▪	Participated in the State Grid Jiangxi Electric Power Company’s line loss APP development project, developed the substation view module to monitor anomalies, display the causes of anomalies and the line loss rate in the substation, etc.<br>


Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
