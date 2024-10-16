# 3DOF Planar Manipulator Control with Reinforcement Learning

This project demonstrates the control of a 3-degree-of-freedom (3DOF) planar manipulator using Reinforcement Learning (RL) techniques. The goal is to control the manipulator to reach a desired position while avoiding obstacles and optimizing movement efficiency. The RL algorithm is implemented using Python and the stable-baselines3 library, with simulation and visualization in an OpenAI Gym environment.

## Project Overview

- **Manipulator**: A 3DOF robotic arm that operates in a 2D plane.
- **Objective**: To control the arm’s end-effector to reach a target position while avoiding a barrier.
- **Method**: The project uses a model-free RL approach, specifically Proximal Policy Optimization (PPO), to learn the control policy.
- **Simulation**: Implemented using Python, Gym, and stable-baselines3. The environment includes visualizations for the manipulator’s movements, target, and obstacles.

## Key Features

- **Custom Environment**: A Gym-based environment is created to simulate the 3DOF manipulator, define the action and observation spaces, and implement reward functions for RL training.
- **Reinforcement Learning**: The PPO algorithm is used to train the manipulator to minimize the distance to the target while penalizing excessive torque and time spent.
- **Collision Avoidance**: The environment includes an obstacle, and the reward function encourages the arm to avoid it while reaching the goal.
- **Visualization**: A graphical representation of the manipulator, target, and obstacle is updated at each step, showing the progress of the manipulator as it moves towards the target.

## Setup Instructions

1. **Clone the repository**: 
   ```bash
   git clone https://github.com/yourusername/3dof-planar-manipulator-rl.git
