---
layout: post
title: "Pixel Race"
date: 2016-12-02
excerpt: "A vintage racing game on FPGA board for UCLA CSM152A."
project: true
tags: [Verilog, FPGA]
feature: https://raw.githubusercontent.com/jmzheng1028/jmzheng1028.github.io/master/assets/img/PR.PNG
comments: false
---



### *Description*
Overview: A vintage racing game on FPGA board. The building process of the project includes designing the overall game logic and the programming of individual Nexsys Board components: buttons for controlling, VGA adapter for displaying the game interface and the Seven Segment display for showing the game score. 

<figure>
	<center><img src="https://raw.githubusercontent.com/jmzheng1028/jmzheng1028.github.io/master/assets/img/Pixel_race_schematic.png"></center></figure>
This top-level shematic shows the main modules responsible for the game logic.

Language: Verilog


### *Insipiration*
This is a FPGA version of the racing game on retro handheld game consoles back in the 90's, a game that my lab partners and I have all played as children. 

One main modification from the console version is the control of the car. The control is no longer discrete: you can held down the right button to gradually move the car to the right at a constant speed, instead of a discrete "jump" to the right lane as in the console version. Also, this FPGA version of the game is no longer black and white: the VGA display adapter of the board is utilized to make the game more colorful.

### *Freatures*
* The player can control a small racing car to move left or right on a track with 3 lanes by using the board's control buttons. 
* Obstacle car will appear and block one of the lane randomly.
* The game will terminate if the player hits any obstacles, and will keep running if the player survives the traffic.
* As the player survives longer in the game, the difficulty of the game increases as the speed of the overall traffic increase. 
* Scores will be displayed on the seven segment display section of the FPGA board.


### *Links*
Check out the video demo of the game: 
<iframe width="560" height="315" src="https://www.youtube.com/embed/-wsM9rczjNI?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>
You can also view this project in its <a href = "https://github.com/jmzheng1028/CSM152A-Lab4" target="_blank"> github repository </a>.
