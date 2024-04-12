# Unity Rover

This repository contains the files developed during the Year 2 End of Year Project (ELEC50008/ELEC50003). The Unity Rover is produced by group IC-CPA2. The project involves several key constituents to be able to simulate a robot which is capable of making autonomous exploration decisions based on the inputs it received through sensors. Here, the constituents include a vision recognizer to identify shape, type and colour of objects as well as a command web-application which sends movement commands through the front end for control of the rover and to display the progress of the mission of a map. Additionally, we had an energy subsystem to enable the battery pack to be powered by solar panels, drive subsection to ensure the rover can drive in a straight manner and turn angles accurately, with a control subsystem to run an arena traversal algorithm and report data through wifi and internet protocols (TCP-IP) to the web-application. 

**A short video demonstrating the rover's ability to drive straight, turn and identify objects and walls is provided below :**

https://user-images.githubusercontent.com/73653114/182037953-e8d1f93e-0e0c-4b1b-aa35-7ad135c4f402.mp4

## Contributors

Our work was coordinated using a flat structure to improve communications and creative thinking. Here, each member decided which subsystem they primarily wanted to develop with all team members working together to integrate the subsystems. The sections each member worked on is written below. 

James (Command & Control),
Matthew (Control & Vision),
Charmaine (Command & Control),
Himanish (Vision),
Milan (Control & Drive),
Kelvin (Energy),
Amy (Drive & Radar)

## Drive Subsection Notes
Please install on platform.io (MFRC522), Wifi (Jake Merz), Sparkfun libraries onto system. Start by running the server by running python/python3 server.py. Then input the values to be input into control the rover. The documentation is expressed in quite an easy readable way.

## Command Subsection Notes
The Command subsystem allows the users to control the motion of the rover through a web application and also displays data retrieved from the rover. It consists of a database in django which stores tile information amongst other map attributes and uses frontend technologies (HTML,CSS, Javascript) for displays and backend technologies in python for processing.  

## To run the code:
```bash 
##all code and dependencies
launch.sh &lt;ip address>
##to run the web application <br>
clear.sh
##To clear database 
```
Windows or MAC OS:
```bash
python manage.py runserver 
# Entering this command in the terminal will suffice. 
```
## Radar Subsection Notes

The purpose of this subsystem is to use the HB100 Doppler radar module to detect a rotating fan located underground. A reflected harmonic signal should be received when the rotating fan is under the rover. The radar developed is fully operational and functional (sample code has 2V tolerance on radar) with the code primarily contained in a radar.h file, however, this code was not integrated fully with other subsystems (as it was not required on demonstration). 

## Software Distribution 
If you wish to use this software please cite it as follows 
```bash
@software{Unity_mars_rover,
  author = {Ong, James and Setiawan, Matthew and Louie, Charmaine and Mang, Hao Jian and Joshi, Himanish and Paczai, Milan and Yau, Amy },
  month = {07},
  title = {{Unity Mars Rover Assembly}},
  url = {[https://github.com/github-linguist/linguist](https://github.com/JamesOngICL/Unity-Mars-Rover)},
  year = {2022}
}
```
