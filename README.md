# Non-parametric model (NID) feedforward control deplyment on the real robot

https://github.com/EduardoRosLab/Baxter_Dynamic_Model/assets/45313868/53a87512-1da1-4947-ba22-3ba1d0be5a56  

The video depicts the Baxter controlled by the NID neural network in a feedforward loop. We
compared the NID performance (accuracy) to a conventional PD. We also compared their performances
under perturbations. We finally showed NID ability to track the reference trajectory
in the absence of active feedback control.

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




