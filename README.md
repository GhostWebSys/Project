# Environment
* ### Ubuntu 18.04
* ### ROS melodic
* ### python3
* ### joystick (Logitech Joystick F710 - D mode)
* ### xdotool

# Introduction
* ### This file is use xdotool package.
* ###  ROS (send joystick msg) -> this file (joystick msg receive and convert. and send key msg.) -> LG SVL Simulator

# How to use.
* ### 1. Install xdotool package.
  ####  If it is installed, skip this step. 
  ####  $ sudo apt-get install xdotool
* ### 2. ROS(melodic) start
  * ####  2-1. Ros start.
    ####     $ roscore
  * ####  2-2. joystick change chmod 777 js[x] ([x] is joystick device number)
    ####     $ sudo chmod 777 /dev/input/js0
  * ####  2-3. joy_node start.
    ####     $ rosrun joy joy_node
* ### 3. LG SVL simulator start.
* ### 4. run this file and control joystick.
  ####   $ python3 joy_control_lgsvlsim.py
