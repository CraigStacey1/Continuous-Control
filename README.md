# Consinuous Control Project
## This repository outlines the steps taken to resolve the Condinuous Control Reacher environments using Unity ML-Agents and Pytorch.

# Environment Setup
## Anaconda
In order to set up the environment follow the instructions on the Udacity deep reinforcement learning course.

https://github.com/udacity/deep-reinforcement-learning

## Reacher Environment for unity
The reacher environment for the continuous control task can be setup by following the instructions on the git-hub page for the continuous control project:

https://github.com/udacity/deep-reinforcement-learning/tree/master/p2_continuous-control

# Running The Agent
In order t orun the agent jupyter notebooks is needed the best way to set up teh environment is to insall anaconda: 
https://www.anaconda.com/distribution/

After creating the environment and downloading the Unity environment open the ContinuoutControl.ipynb file in anaconda and run all cells of the notebook.

# Learning Agent
The learning agent used for this project is a Deep Deterministic Policy Gradient agent. This agent uses 2 neural networks known as the Actor network and the critic network. The actoor network performs actions based off the current policy, producing the actions directly instead of producing probabilities. The Critic network provides feedback on the performance of the actor network in orrder to improve the Actors policy.

## Neural Netsork Structure
Both the actor and the critic have the same internal hidden layer values in this project, however the output layers differ

- Input: State Size = 33
- Hidden Layer 1 = 512
- Hidden Layer 2 = 512

- Output layer Actor: Action Size = 4  (Maps the states to actions)
- Output Layer Critic: 1 (maps the (state, action) pairs to Q-values)

# Results

The graph below shows the results of the training of the agent.

![](results/ScoreImage.png)

As can me seen the score goes above 30 at episode 40 and remains there for the next 110 episodes




