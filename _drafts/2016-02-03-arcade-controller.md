---
layout: 	blogpost
size:     s
title:  	"Building an arcade controller with Arduino"
tags:   	games electronics build-logs
excerpt:	|
  A build log of the arcade contoller I built using a fake Arduino, off-brand controller parts and love.
colour:		"#0EC5E9"
---

Costs:
======

Notes:
======

Set up Arduino and python environment on Windows.
Serial chip had problems with communicating with PC (USB 3.0 problem)
Testing simple 2 switches with wire and resistors, sending byte to represent switch state, using pywin32 to send keystrokes based on switch state
Got most of the code working pretty easily (but why are bytes being sent in the wrong order? That's weird)
Hooked up a joystick, that works... but MAME uses DirectInput! Change from winapi to sendkey... but MAME uses DI in raw mode! Compile MAME to use normal DI instead  of raw mode (used .
Worked! Played Pac-Man. Tried winapi32 again, but super laggy. Using the sendkeys code

Switched to using internal pull-up resistors - woohoo, now I don't need to worry about supplying 5V to 26 different input pins!
Wired up all player 1 controls using header pins. 
Lots of play testing!