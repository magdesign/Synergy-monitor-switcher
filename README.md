# Synergy-monitor-switcher
Switch display input source with Symless Synergy tool



Tested on Ubuntu Linux.
Does not seem to work with Nvidia in combination with DP ports, but test for yourself.
Mine jsut works from switching DVI to DP, switch back has to be done manually.

Change the path to your own synergy.conf file.


For my dell monitor, I figured out:

Switching to DP:
 sudo ddccontrol -r 0x60 -w 15 dev:/dev/i2c-3
 
 Switching to DVI:
  sudo ddccontrol -r 0x60 -w 14 dev:/dev/i2c-3


No support.
Use the code as you want.
©2018 magdesign.ch
