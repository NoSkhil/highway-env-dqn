Autonomous Driving Optimization using Reinforcement Learning

This project implements reinforcement learning to develop autonomous driving agents that optimize vehicle routing and lane management while adhering to safety thresholds. The project uses Highway-Env's 2D simulation environment to train decision-making agents that can adapt to diverse traffic patterns and make intelligent decisions in complex driving scenarios.

Team Members
- Shyam Akhil Nekkanti
- Layanika V.S
- Samyukth Lalith Lella Gopal

Project Overview

Traditional autonomous driving approaches face two critical challenges:
1. Limited adaptability to diverse traffic patterns
2. Poor decision-making in complex driving scenarios

Our DQN-based solution learns optimal driving policies through direct interaction with simulated environments, eliminating the need for labeled data.

System Architecture

- *Environment*: Highway-Env Simulator with vehicle states, actions, and reward mechanisms
- *DQN Algorithm*: Neural network with experience replay, custom reward function, and target networks
- *Evaluation*: Safety performance, efficiency metrics, learning stability, and policy visualization

Features

- *Enhanced Neural Network*: Multi-layer architecture for Q-value function approximation
- *Custom Reward Function*: Balances safety and efficiency using distance and velocity parameters
- *Epsilon-Greedy Exploration*: Adaptive strategy for balancing exploration and exploitation
- *Performance Visualization*: Live-updating plots for tracking training progress
Installation

1. Clone this repository:
bash
git clone https://github.com/yourusername/autonomous-driving-rl.git
cd autonomous-driving-rl


2. Install dependencies:
bash
pip install -r requirements.txt


Usage

Run the Jupyter notebook to train and evaluate the agent:
bash
jupyter notebook RL_Final_Presentation.ipynb


Evaluation Metrics

We evaluate our RL agents based on:
1. Safety performance (collision avoidance rate)
2. Efficiency metrics (travel time, speed maintenance, lane discipline)
3. Scenario completion rate at different traffic densities
4. Training convergence speed
5. Generalization across different Highway-Env scenarios

Results

The DQN agent demonstrates:
- Effective collision avoidance in most scenarios
- Appropriate speed management in varying traffic conditions
- Strategic lane changing for optimal driving
- Gradual reward improvement over training episodes

Project Structure

- RLFinal-Group1.ipynb: Main notebook with implementation and visualization
- *requirements.txt*: Required packages for running the code
- *models/*: Saved model checkpoints
- *gifs/*: Generated visualizations of trained agents

Future Work

- Implement and compare PPO and A2C algorithms against DQN performance
- Test on more complex scenarios such as merge-v0 and intersection-v0
- Develop custom scenarios with varying traffic densities
- Implement automated hyperparameter optimization for reward function tuning

License

This project is licensed under the MIT License - see the LICENSE file for details.

 Acknowledgments

- Highway-Env team for the simulation environment
- PyTorch team for the deep learning framework
