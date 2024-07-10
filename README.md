# Move-the-robot
These steps are an algorithm for operating servo-tensor type motors to produce the walking motion of the robot
## 1. Initialize Joint Angles:
- Determine the initial angles for the robot's joints and store them in the` joint_angles` variable.
 
 ## 2. Define the Walking Cycle:
 - Identify the target joint angle values for each step of the walking cycle and store them in the` walk_cycle` variable.

 ## 3. Repeat the Walking Cycle:
 - Repeat the following steps to go through each step in the walking cycle:

   ### 1. Update Joint Angles:
   Update the `joint_angles` values according to the target values in the current step of` walk_cycle.`
   ### 2. Set Servo Angles:
    Adjust the servo motor angles for each joint according to the current `joint_angles` values using the `set_servo_angle()` function.
   ###   3. Control DC Motors:
   Adjust the speed of the DC motors for forward motion using the` set_motor_speed() `function.
   ###  4. Add Delay:
   Add a delay between steps to ensure smooth motion.

## 4. Stop the Motors:
- When the walking cycle is complete, stop the DC motors using the `set_motor_speed()` function.

