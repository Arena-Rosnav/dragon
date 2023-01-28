# DRAGON

DRAGON is ROS navigation approach created by [Autonomous Mobile Robot Lab at University of Virginia](https://www.bezzorobotics.com/).  
This repository extends the original work by integrating it into arena-rosnav.  
For original work refer [here](https://github.com/nocholasrift/UVA-AMR-BARN--ICRA2022).


# Installation
## Add this package to your .rosinstall or clone it manually.
```bash
cd ~/catkin_ws/src/arena-bench # Navigate to your arena-bench location
echo "- git:
    local-name: ../planners/dragon
    uri: https://github.com/Arena-Rosnav/dragon
    version: master" >> .rosinstall
rosws update ../planners/dragon # or rosws update
```
## Activate poetry shell
```bash
cd ~/catkin_ws/src/arena-bench # Navigate to your arena-bench location
poetry shell
```
## Make sure to source the workspace environment
```bash
cd ../.. # navigate to the catkin_ws directory
catkin_make
source devel/setup.zsh # if you use bash: source devel/setup.bash 
```
# Usage
## This planner can be chosen using the local_planner argument like so:
```bash
roslaunch arena_bringup start_arena.launch local_planner:=dragon # Make sure that your virtual env/poetry is activated
```
## For more details regarding usage, please refer to our [documentation](https://arena-benchmark.readthedocs.io/en/latest/user_guides/usage/)
