Web based interface for controlling the Raspberry Pi Camera, includes motion detection, time lapse, and image and video recording.
Current version 6.6.26
All information on this project can be found here: http://www.raspberrypi.org/forums/viewtopic.php?f=43&t=63276

The wiki page can be found here:

http://elinux.org/RPi-Cam-Web-Interface

This includes the installation instructions at the top and full technical details.
For latest change details see:

https://github.com/consiliumsolutions/RPi_Cam_Web_Interface/commits/master
  
This version has updates for php7.3 / Buster. May need further changes for nginx

**NOTE: This version of RPi_Cam_Web_Interface includes a precompile rpicam-mjpeg binary to be used with the web interface. This is meant to replace the now-outdated RaspiMJPEG that was previously included. Users have reported issues with using the precompiled binary, and so you may need to rebuild rpicam-apps from source.**

If you need to build rpicam-apps, follow the instructions in [README_rpicam-apps.md](README_rpicam-apps.md). This repository contains the source code of the rpicam-mjpeg fork of rpicam-apps.

# Basic Installation
Assuming the precompiled binary of `rpicam-mjpeg` works for you, you will only have to run `sudo ./install.sh` to install the web interface. `gpac` was a dependency of the old RPi_Cam_Web_Interface, however this is no longer available via `apt`, so must be built from source. If your computer already has `gpac` installed, then you can change this option to "no" in the installation dialogue.

# Basic Usage
After installing, either select start web interface or run `sudo ./start.sh` after installation to start RPi_Cam_Web_Interface. Navigate to http://\<your ipv4>/html on any device in your network to gain access to the web interface.

A more detailed usage guide is available on the [web interface wiki](http://elinux.org/RPi-Cam-Web-Interface)