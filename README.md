# DRAGON

DRAGON is ROS navigation approach created by [Autonomous Mobile Robot Lab at University of Virginia](https://www.bezzorobotics.com/).  
This repository extends the original work by integrating it into arena-rosnav.  
For original work refer [here](https://github.com/nocholasrift/UVA-AMR-BARN--ICRA2022).


# Installation

## Activate poetry shell
```bash
cd arena-rosnav # navigate to the arena-rosnav directory
poetry shell
```
## Make sure to source the workspace environment
```bash
cd ../.. # navigate to the catkin_ws directory
catkin_make
source devel/setup.zsh # if you use bash: source devel/setup.bash 
