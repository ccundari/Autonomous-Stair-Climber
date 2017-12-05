# Autonomous-Stair-Climber
  LabView control code for a robot that is designed to navigate a course that includes climbing and descending stairs and avoiding obstacles.

  There are two control modes. Manual operation has the operator controlling the robot from a remote location over a wireless network connection. The operator recieves real-time video feed from the webcam mounted on the front of the robot.
  
  Autonomous operation has the robot operating independently. The course has yellow arrows spaced ten feet apart, and obstacles (large cardboard boxes or similar) blocking this path. The webcam on the front of the robot tracks the yellow arrows and steers the robot to follow them. Ultrasonic sensors around the robot will override the path following if an obstacle is detected, and navigate the robot past the obstacle and help the webcam reaquire the original path.
  
  In both modes there is a pitch check that constantly analyzes if the robot is attempting to ascend or descend stairs. If the robot enters this mode, the onboard accelerometer is used to guide the robot, and prevent tipping to the right or left if the obstacle is not completed evenly.
