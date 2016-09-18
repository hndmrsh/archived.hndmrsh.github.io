---
layout: 	blogpost
size:     l
title:  	"Arcade Box part 2: Baking some Pi"
tags:   	games electronics build-logs
excerpt:	|
  Setting MAME and the control panel up on the Raspberry Pi
colour:		"#0EC5E9"
---


Notes
=====

- Need to decide which distro to go with: naturally I want power and customization, so I'll go as minimal as possible - is Arch avaiable on Pi?
    - Yep: https://archlinuxarm.org/platforms/armv8/broadcom/raspberry-pi-3
    - Followed instructions to install on a 2GB SanDisk microSD card
    - Got it booting with a 1A phone charger, but this will probably have to be replaced to run MAME
    - Now need to set up WiFi and start
      - Managed to connect to my wireless network with wifi-menu, which set up a daemon (so should automatically reconnect on boot)
    - Mount external HDD by adding it to fstab
      - Installed ntfs-3g so I can mount it
      - Added the external drive to fstab mounting with user permissions for the default Arch Linux ARM user ("alarm")
    - Need to now install MAME and copy over romset
      - Going to go with a libretro setup to start with; probably going to need to download a fresh romset to be compatible with lr-mame2003 though (based on MAME 0.78)
    - ssh'd into the Pi, installed alsa-utils so I could test the sound
      - alsa-utils required libsndfile-1.0.26-1-armv7h.pkg.tar.xz, mirrors only had 1.0.27; found another mirror with the right file and added to mirrorlist
      - Installed mpg123 to test audio playback; works fine!



Resources
----------
https://github.com/retropie/retropie-setup/wiki/Managing-ROMs : managing the ROM set with ClrMAMEPro
