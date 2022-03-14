when the ball is shot from the robot, the ball will have a force given to it by the robot's velocity in the directoin of the robot heading. the turret angle and the flywheel speed will give the ball another force. the goal is that the robot is to give the ball a velocity in the correct directoin for the ball to go into the target.

first step is to calculate a velocity and angle for the ball to shoot at for the robot to hit the target without a motoin from the robot. we will add compinsatoin for robot motoin after.

the target is at a fixed positoin and the ball will travel in the arc of a negative parabola

first step is calculate this arc given a robot with 0 velocity in any direction and assuming that the robot's turrret is facing correctly.                                                                               

this can be expressed in a 2 dimentional place where y is the distance from the ground and x is the distance the robot is from the target. this plane can be revoluted around the goal to make sense in a 3 dimentional sense.

## how to calculate velocity from a stopped position
assuming that the drivetrain of the robot and the turret are in the same xy positoin (which isn't true)
the turret is at a fixed angle for now and we can later add the funcitoinality to to find the most optimal ball path once we have an adjustable shooter hood.

the equation for the velocity of the ball with a fixed angle and a fixed target is:
V = ((horizontal distance to target) * sqrt(-gravity)) / 
(sin(launching angle) * sqrt(-2 * (height to the target - (horizontal distance to target/tan(launching angle))))

{https://www.desmos.com/calculator/c2tdl39fhb - derived by josiah fu}

now with the equation for velocity given a launch angle (constant), distnance to target vertically (constant), and a distance to target horizontally (variable), we can 