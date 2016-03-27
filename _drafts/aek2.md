---
layout: 	post
title:  	"Restoring an Apple Extended Keyboard II"
date:   	2016-02-01 17:55:00 +1300
categories:	electronics build-logs
---

Costs:
======

Keyboard: $10
Converter:
 Teensy: $40 (incl. shipping)
 Case: $1.90
 4 pin mini-DIN (S-Video) jack: $3.50


Notes:
======

Stage 1: Getting it working
---------------------------

Started looking for vintage keyboards (esp. Model M), found an AEK1 on TM.
Discovered the GeekHack page and related GitHub repository.
Lost bidding at $24. Found an AEK2 in better condition following week for a $10 BN!
Felt great to type on, so...Bought a Teensy online.
Took home, but got confused with terminology and software!
Downloaded Make for Windows, seemed to work. Tried dfu_programmer, but didn't seem to be what I wanted.
Discovered I needed the AVR toolchain to compile the firmware.
All seemed to be OK, but wasn't compiling! Make was having trouble with the AVR GNU compiler.
Found people seemed to like using MinGW to compile this firmware, so downloaded that.
Had to add Make and the AVR compiler to the MinGW PATH env var.
Managed to finally get it compiling with these commands:
  make clean
  make -f Makefile.teensy teensy
Needed to load it into the teensy firmware - make threw up some errors about not finding dfu_programmer - why? (probably because I never added it to the path, but documentation suggested I shouldn't be using it for Teensy anyway).
Downloaded teensy_loader_cli and added that to the PATH.
Installed firmware with:
  teensy_loader_cli
Eureka!

Stage 2: Customise the firmware
-------------------------------

Didn't like the way Option was mapped to Alt and Command was mapped to Windows - technically correct, but not natural for Windows keyboards.
Wanted media keys, so mapped to F1--F4
Wrote custom keymap and modified MAKEFILE.
Updated firmware with:
  make clean
  make -f Makefile.teensy teensy KEYMAP=hndmrsh

Stage 3: Pretty it up
---------------------

Created Retr0bright mixture, used to de-yellow case and spacebar?
Cleaned keycaps (soap?), tidied between switches with cotton buds?







NB to add to software page:
===========================

Compilation now includes the teensy_loader_cli command, compile and install firmware with:
  make clean
  make -f Makefile.teensy teensy KEYMAP=hndmrsh