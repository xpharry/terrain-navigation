# sentry_urdf (modified from mobot_urdf)
Contains sentry.xacro model of wheelchair-like robot.  Also has a launch file.

## Example usage
Start gazebo with an empty world:

`roslaunch gazebo_ros empty_world.launch`

then load the robot model into Gazebo via the parameter server:

`roslaunch sentry_urdf ground_plane_with_sentry.launch`

Drive the robot around, e.g. with:

`rostopic pub cmd_vel geometry_msgs/Twist  '{linear:  {x: 0.5, y: 0.0, z: 0.0}, angular: {x: 0.0,y: 0.0,z: 0.3}}'`

Launch file for this example does not include joint-state and robot-state publishers for use with rviz.

    
