# Forward-Kinematics-Solver

## Project Description
The project involves creating a Forward Kinematics Solver for a robot arm. It implements the kinematic analysis of the UR10 and Franka Emika Panda robotic manipulators using the Denavit-Hartenberg (DH) convention. It calculates transformation matrices for different robot configurations and determines the position of the end effector.

## Dependencies
* Python 3.11 (any version above 3 should work)
* Python running IDE (I've used Pycharm)

## Libraries used
* SymPy

## Instructions
1. Download the zip file and extract it
	
2. Install python and the required dependencies: 

   * From the terminal in your IDE, run the following commands:
     
      `git clone https://github.com/sympy/sympy.git`

      `git pull origin master`

      `python -m pip install -e`
	
4. Run the code or use desired python IDE:

	`$python3 Fkinematics_solver.py`

  To successfully run the code, give each joint angle and press 'Enter', till 6 joint angles (from 0 to 5) are obtained. For example, if you want the robot in 'Home configuration', enter the following joint     angles [0,0,0,0,0,0]

  Note* Please enter 'int' or 'float' values. 'string' values like 'pi' or 'pi/2' would display an error

## How it works

* The program constructs the homogeneous transformation matrix for each joint.
* It multiplies the matrices to obtain the final transformation from the base to the end effector.
* Users can input custom joint angles to compute the kinematic configuration.
