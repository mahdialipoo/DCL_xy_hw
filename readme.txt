Control the position of the robot and bring the robot to a non-aligned point
In the relevant code, the movement of the robot in a هدdirect path is controlled by implementing the PID class.This is impelimented in PID.py .
The P controller has low speed and accuracy because its speed decreases as the robot approaches the desired state.
The integrator is used to improve the accuracy and the derivative is used to improve the speed of reaching the desired state.
Due to the derivative property in increasing noise, a filter has been used next to it.
All controllers are discrete by the backward discretization method.
In this way, the iddar controller may become unstable, but instability does not become stability.
The dead zone effect is applied by the section specified in the code. This phenomenon did not exist in the simulation. If the wheel speed is less than 0.1 m / s, the engines will enter the dead zone and the speed will be zero.


