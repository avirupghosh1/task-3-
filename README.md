
# Task-3(A)

Aruco detection in real world and gazebo world(through robot camera pluggin)

gazebo world detection
-
- first create a workspace and a src directory in it then clone the git repo
```bash
git clone https://github.com/avirupghoshiitmandi/task-3-.git
```
- build your workspace with catkin_make
```bash
 cd ..
 catkin_make
 ```
 - now launch the bookstore world with few aruco markers (using args = "DICT_6X6_1000")
 ```bash
  roslaunch turtlebot3_gazebo turtlebot3_world.launch
  ```
  - now to move your bot launch the teleop node
  ```bash
  roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
  ```
 -  and at last to see the camera output and the detection of aruco markers run the aruco.py script and also make the python file executable first.
 ```bash
  cd src/aruco_script/src
  chmod +x aruco.py
  cd ..
  cd ..
  cd ..
  ```
 ```bash 
 rosrun aruco_script aruco.py
 ```
 you will be able to see the arucomarkers getting detected(the markers near left end skyblue window are most properly detectable as there is no bright white or dark black areas nearby I have tried to put some markers in the middle along with adjusting the light but the detection oscilates meaning it flickers through the frames )

THE TASK3 1ST PART WITH REAL LIFE DETECTION IS IN THE TASK3B REPO!!
