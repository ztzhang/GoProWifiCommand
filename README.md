# GoProWifiCommand
Gopro wifi command hack---a sniff result of Gopro App . 
The Json file can be used as a Gopro control API. 
Simply connect to yout Gopro hotspot and send the corresponding http request to control it via Wifi. Only Tested for Hero4.

#Known Issues:
Change to submode commands, ie, change to timelapse multishot, do not work. The sniff result are correct, but would return 400 if tested on PC. A ugly solution is to change default mode and submode, then perform sleep+wake.
If your are experiencing unstable wifi connection, or unexpected time out from camera, please try issuing a GetStatus request every second or so, it would greatly improve the connectivity mysteriously.

#MISC:
I also worte a wificontroller and camera controller module in python, but only work under windows. It is designed to control multiple gopro cam(16 in my case) simutaneously using extra wifi interfaces. I also had a GUI for that, if you need those code, please contact me: gatzbutnotgreat at gmail dot com.

#Reference:
https://github.com/KonradIT/goprowifihack: KonradIT's version seems a bit outdated. Different urls are used to control the same property in diffrenet modes, ie, Video, Photo, Multi-Shot.
