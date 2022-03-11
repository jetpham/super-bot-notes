#### inputs
- vision
	- distance of the target
	- angle to the target
- odometry
	- position of the robot
	- velocity of the robot
	- angular velocity
	- heading of the robot
- turret
	- turret heading
	- it is important to note the limits that the turret has for shooting
- flywheel
	- the current rpm of the flywheel
	- it is important to note that limits that the flywheel has including the maximum rpm, max acceleratoin, and max deceleration

#### output
- turret
	- turret angle
- flywheel
	- flywheel rpm
- leds
	- create a command that returns the state that sotm is in
- simulation
	- give turret angle, flywheel rpm, and led state to the sim