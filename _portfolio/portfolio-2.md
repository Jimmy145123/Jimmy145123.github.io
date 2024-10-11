---
title: "KOREN Net Challenge Season 11"
excerpt: "Developed a drone control system for collision avoidance through network establishment. <br/><img src='/images/KOREN.jpg'>"
collection: portfolio
---

As the team leader of the \'Sky Guardians\', our topic was selected as finalist for [KOREN Net Challenge Season 11](https://www.koren.kr/kor/Alram/contyPass.asp?cd=34&page=1). Our team anticipated the future commercialization of drones for services like drone delivery and drone taxis, and developed a drone control system to ensure safe flight operations. Utilizing the KOREN network and Virtual Machines, we enabled communication between drones and a central server. Click [here](/files/최종발표자료_스카이가디언즈.pdf) to view related documents of our topic and [here](/files/최종평가시연동영상_스카이가디언즈.mp4) for demonstration video.


In the competition, I noticed the growth potential of the drone market and proposed the idea of a drone control system. I took part in planning the flight of the drone using the ArduPilot drone simulator and wrote the drone avoidance code. <br/><br/>

<img src='/images/ardupilot.png'><br/>ArduPilot program is a drone flight simulator that can connect a real drone, set its flight path, and make drone automatically fly along the flight route. Although our team was unable to purchase a real drone due to budget problems, we used \'Simulation\' mode in the ArduPilot program to plan the flights of virtual drones within the software. Through this program, we were able to get flight data(Drone battery, flight speed, altitude) from the virtual drones using MAVLink program.<br/><br/>

<img src='/images/avoidance.png'><br/>I wrote a Python program where users can input the number of drones, along with the departure and destination latitude, longtitude for each drone. The program assesses the possibility for collisions between drones and adjusts their departure times accordingly. I assumed that all drones travel at the same speed, so the program measures the distance between drones over time. If the distance falls below a certain threshold, the program assumes a collision and delays the departure time of the drones by one second.



