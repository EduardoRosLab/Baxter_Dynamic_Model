# Dataset Baxter robot

This dataset contains the training and test 
data that were used for the recurrent neural
network to learn the inverse dynamics of the 
Baxter robot.

The data correspond to the angles and 
velocities of the joints when a torque 
is applied in order to follow a trajectory.

## Trajectories

* Random: The desired trajectory is random 
           points in the robot's workspace.  
           
* sin_XYZ_(Tt)s_T(Txy)_Tz_(Tz)T_r(r): 
           The desired trajectory is defined 
           by sinusoids in x, y and z.  
           
           * Tt: total period [seconds]  
           
           * Txy: Period in xy [seconds]  
           
           * Tz: period in z [Txy]  
           
           * r: radius in XY [cm]  
           
* spiral: The desired trajectory is a spiral
           with radius in XY depending on 
           time [r(t) = kt].

## Data description

1:7   joint angles, from s0 to w2  

8:14  joint velocities, from s0 to w2  

15:21 joint torques, from s0 to w2
