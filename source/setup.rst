.. _setup:

Developer Environment Setup
===========================

Setup the development build environment. You can use the pre built virtual macihne that is
already setup and configured for a developer. If you like, you can also follow the instructions
below to create a new instance.

Virtual Machine
===============
Prebuilt image for Stampede Robotics developer
* Download and Install the latest version of VirtualBox by Oracle
* Download virtual image
* Create new virtual machine and use existing vm.

Manual Build
============
Setup the development environment step by step manually. 

Install Operating System
------------------------
* Install latest stable lubuntu release
* sudo apt update
* sudo apt dist-upgrade


Install Software
----------------

Install GCC/G+
++++++++++++++
* sudo apt install build-essential

Install Python 3.6
++++++++++++++++++
* sudo apt install python3.6
* cd /sr/bin
* ln -sf python3.6 python3
* ln -sf python3.6m python3m

Install App Dependency
++++++++++++++++++++++
* sudo su
* apt install libgconf-2-4
* apt install git
* apt install python3-pip
* apt install python3-setuptools
* apt install python3-pytest
* apt install python3-logilab-common
* apt install libsdl2-developer

Install Python Library Depdency
+++++++++++++++++++++++++++++++
* sudo su
* pip3 install --upgrade pip
* pip3 install pygame
* pip3 install sphinx_rtd_theme
* pip3 install sphinx 
* pip3 install pyqt5

Install Editor
++++++++++++++
* download latest visual editor at https://code.visualstudio.com
* sudo su
* dpkg -i latest.deb
* apt install -f 
* apt update
* apt install code

Install QT5
+++++++++++++
* download latest from https://www.qt.io/download/
* chmod a+x qt-unified-linux-x64-2.0.5-online.run
* run the file ./qt-unified-linux-x64-2.0.5-online.run
* sudo apt install qtchooser
* sudo qtchooser -install Qt5 /opt/Qt/5.8/gcc_64/bin/qmake

Install RobotPy
+++++++++++++++
* sudo su
* pip3 install pyfrc
* mkdir robotpy
* cd robotpy
* git clone https://github.com/robotpy/examples.git

Install QDriverStation
++++++++++++++++++++++
* git clone https://github.com/FRC-Utilities/QDriverStation.git
* cd QDriverStation
* sudo su
* qmake -qt=Qt5
* qmake
* make install


