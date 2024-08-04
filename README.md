# TurtleBot3-Navigation
Using TurtleBot3 packages to navigate a robot into simulation world
<h2>Setup</h2> <br>
start by setting up the workspace enviroment <br>

1- ```mkdir -p ~/test_turtlebot/src``` <br>

create a new workspace <br>
2- ```cd ~/test_turtlebot/src``` <br>

get inside your workspace src file to start cloning clone packages. <br>
<h2>install packages</h2> <br>

1- ```git clone http://github.com/ROBOTIS-GIT/turtlebot3.git``` <br>

2- ```git clone http://github.com/ROBOTIS-GIT/turtlebot3_msgs.git``` <br>

3- ```git clone http://github.com/ROBOTIS-GIT/turtlebot3_simulation.git``` <br>

![turtlebot catkin setup](https://github.com/user-attachments/assets/7c75b3d0-c5af-4132-94a0-c537ad3fa537) <br>
now go back to your workspace using `cd catkinn` command,and run: <br>

`catkin_make` <br>
to clone packages. then source your terminal using:<br>

```Source ~/test_turtlebot3/devel/setup.bash``` <br>

```Export TURTLEBOT3_MODEL=burger``` <br>

here we are telling the terminal that we’re using the burger model from our packages.<br>
now we will run our gazebo world: <br>

```roslaunch turtlebot3_gazebo turtlebot3_world.launch``` <br>
![turtlebot roslaunch](https://github.com/user-attachments/assets/8ee188ab-500d-4c23-8de3-43dd8661ac02)
<br>
![turtlebot gazebo world](https://github.com/user-attachments/assets/3af31df6-03db-42e6-95ee-4b508bcd4914)

<br>
<h2>Robot Motion</h2> <br>
Now to start moving your robot model, open a new terminal window (from top left cornor) <br>
and start by sourcing this session again using:

```Source ~/test_turtlebot3/devel/setup.bash``` <br>

then will introduce our model again to this session using:

```Export TURTLEBOT3_MODEL=burger``` <br>
finally run:

```roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch``` <br>

![turtlebot 2nd terminal setup](https://github.com/user-attachments/assets/81d75821-abd4-41e6-99dc-35d4d5b5515b) <br>
![turtlebot teleop node](https://github.com/user-attachments/assets/2a293b06-378a-45f4-9e67-9312174d2e3e) <br>
![turtlebot teleop2](https://github.com/user-attachments/assets/121193ed-5dcf-452a-9264-db42dfd2529b) <br>
now use your keyboard keys to move your robot model <br>
![turtlebot motion](https://github.com/user-attachments/assets/e1119e1f-e792-47bd-961f-b532aa859fec)
