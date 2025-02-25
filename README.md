# Sample
Overall this is a sample of some projects I have worked on. Typically, I am the only one who has to read it or work with it, but I try to ensure that it is flexible and robust so that in the future, I can simply copy and paste my various functions and classes. This is why certain code blocks repeat themselves across projects.  I write the object once, properly, and then I don't need to worry about it down the road. Also, I ask you ignore the local pathways for backing up my neural network parameters and data. This is to ensure in the event of system crash, I can access the information online and the simulation is not lost. Of course, any reference to these will create an error on your local machine.

## AnnProj
There was discussion at a point in my research where it was thought I may need custom tools beyond that which was provided by deep learning packages like Pytorch. To this end, I wrote my own code to develop and train feed forward neural networks using automatic differentiation as well as the ADAM method for optimization of network parameters. I did this to regress a function for a simple periodic data set. This code should run without any special need for packages.

## RL_CPC
The folder RL_CPC contains the code used for the  publication "Development of algorithms for augmenting and replacing conventional process control using reinforcement learning":
https://www.sciencedirect.com/science/article/abs/pii/S0098135424002448
This code is probably the most disorganized given the number of situations and circumstances I needed to model. Fot that, I apologize. It uses a custom virtual environment based on the IDAES package as well as pyomo and pytorch. There are two files, one containing simulation of a flow sheet of a solid oxide fuel cell, and the other of a continuous stirred tank reactor. In both cases, I needed to simulate conventional control, reinforcement learning control, and dynamic modelling of the system under a number of different disturbances and scenarios.

## AdvisorAlg
The folder AdvisorAlg contains some of my most recent work. This uses state space models of a selective catalytic reduction unit as opposed to a pyomo model. Here you should be able to actually simulate without a custom virtual environment with IDAES downloaded. However, the functions that contain elements of gaussian mixture models have not quite been worked out yet, so I enourage disabling the special_train and special_exp options if you wish to try see the code in action for training.


