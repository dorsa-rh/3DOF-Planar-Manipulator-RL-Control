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



## Environment

- **State**: The state includes joint angles and angular velocities of the three joints, along with the distance to the target.
- **Actions**: The action space consists of torques applied to each of the three joints.
- **Reward**: The reward function is based on reducing the distance to the target, avoiding collisions with obstacles, and minimizing the total torque applied.

## Visualization

- The simulation includes a graphical display of the manipulator, target, and obstacle in the 2D plane.
- The progress of the manipulator’s end-effector towards the target and its interaction with the obstacle is shown in real time.

## Results

- The RL-trained model demonstrates smooth control of the 3DOF manipulator, efficiently reaching the target while avoiding obstacles.
- The performance of the agent improves over time, with decreased movement time and reduced torque application.

## Future Enhancements

- Implement advanced RL algorithms like SAC (Soft Actor-Critic) for improved learning performance.
- Add more complex obstacles and constraints to make the environment more challenging.
- Explore the application of this method to manipulators with more degrees of freedom.

## References

- **Libraries Used**:
  - Gymnasium for environment creation and management.
  - Stable-Baselines3 for RL algorithm implementation.
  - NumPy and Matplotlib for numerical calculations and visualizations.


## Visualization

- The simulation includes a graphical display of the manipulator, target, and obstacle in the 2D plane.
- The progress of the manipulator’s end-effector towards the target and its interaction with the obstacle is shown in real time.
- **Watch the simulation video**: [Watch the video](https://github.com/dorsa-rh/3DOF-Planar-Manipulator-RL-Control/blob/main/Recording%202024-07-10%20143416.mp4)
  
