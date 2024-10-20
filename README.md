# PID_Controller_for_self_balancing_robot
This Repo Demonstrates a self-balancing robot, equipped with an MPU6050 sensor and stepper motors, controlled by a PID controller implemented on an Arduino. The robot reads the tilt angle from the MPU6050 sensor and adjusts the motor speed to maintain balance using a PID Controller.

For more details, you can refer to [this document](https://www.diva-portal.org/smash/get/diva2:1737768/FULLTEXT01.pdf). which has been used as a reference to make this robot
### PID Controller :
A PID controller **(Proportional-Integral-Derivative)** is a control mechanism that adjusts a system's output based on the error between the desired setpoint and the actual process variable. It does so by combining three terms: the **proportional term** reacts to the current error, the **integral term** accounts for the accumulated past error, and the **derivative term** predicts future error by observing the rate of change. The total output is the sum of these three components, given by the formula: 

The PID controller equation used in this project is:

`PID(error) = Kp * error + Ki * integral(e(t) dt) + Kd * de/dt`

Where:
-  **Kp** is the proportional gain
-  **Ki** is the integral gain
-  **Kd** is the derivative gain
-  **e(t)** is the error at time \( t \)

Common tuning methods for adjusting 𝐾 𝑝 K p ​ , 𝐾 𝑖 K i ​ , and 𝐾 𝑑 K d ​ include manual tuning, the Ziegler-Nichols method, and trial and error, each aiming to optimize system stability and response time.

### Realization of the robot :
![Self Balancing Robot](.doc/self_balancing_robot.jpg)
