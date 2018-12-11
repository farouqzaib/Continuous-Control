[//]: # (Image References)

[image1]: https://github.com/Unity-Technologies/ml-agents/blob/master/docs/images/reacher.png "Trained Agent"

# Project 2: Continuous Control

### Introduction

For this project, I trained multiple agents to move to target locations and remain there for as long as possible.

![Trained Agent][image1]

A reward of +0.1 is provided for each step that the agent's hand is in the goal location.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

The task is episodic, and in order to solve the environment, the agents must get an average score of +30 over 100 consecutive episodes.

### Files

- Continuous_Control.ipynb - code for agent
- README.md - this file
- Report.pdf - a report on the algorithm used to train the agent and its performance
- requirements.txt - dependencies required by agent's code
- checkpoint_actor.pth - actor model weights for a agents that successfully solved the control task
- checkpoint_critic.pth - critic model weights for a agents that successfully solved the control task

### Getting Started

NOTE: This code requires Python 3.6

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

2. Place the file in the root directory and unzip (or decompress) the file. 
3. Open Continuous_Control.ipynb and replace `<path to Reacher environment just unzipped/uncompressed>` (in 2. Fetch the environment) with the path to the file from Step 2 above.

### Training the Agent

The code is contained in an interactive notebook, Continuous_Control.ipynb. So all you need to do is run each code cell, one after the other.