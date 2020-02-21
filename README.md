# Udacity deep reinforcement learning project 1 Navigation
In this project, an agent is trained for navigation. And it needs to collect yellow bananas while avoiding blue bananas.

## Environment
Provide a +1 reward to collect yellow bananas and a -1 reward to collect blue bananas. Therefore, the agency's goal is to collect as many yellow bananas as possible while avoiding the use of blue bananas.

### The state space 
State space has **37 continuous dimensions**, including the speed of the agent and the ray-based perception of objects surrounding the agent's forward direction. With this information, the agent must learn how to best choose the action.

### The action space
**Four discrete actions** are available, corresponding to:

- 0 - move forward.
- 1 - move backward.
- 2 - turn left.
- 3 - turn right.

### Solving condition
The task is episodic, and to solve the environment, agent must **score an average of +13 out of 100 consecutive plots.**

## Method details

