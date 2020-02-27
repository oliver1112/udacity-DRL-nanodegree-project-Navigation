[//]: # (Image References)
[gif1]: https://github.com/oliver1112/udacity-DRL-nanodegree-project-Navigation/blob/master/assets/trained%20agent.gif "Trained"
[gif2]: https://github.com/oliver1112/udacity-DRL-nanodegree-project-Navigation/blob/master/assets/random%20agent.gif "Random"

# Deep Reinforcement Learning Project : Navigation
In this project, an agent is trained for navigation. And it needs to collect yellow bananas while avoiding blue bananas.

## Environment
![Random][gif2]
You can see a random agent from the gif. The environment provide a +1 reward to collect yellow bananas and a -1 reward to collect blue bananas. Therefore, the agent's goal is to collect as many yellow bananas as possible while avoiding the use of blue bananas.

### The state space 
State space has 37 continuous dimensions, including the speed of the agent and the ray-based perception of objects surrounding the agent's forward direction. With this information, the agent must learn how to best choose the action.

### The action space
Four discrete actions are available, corresponding to:

- 0 - move forward.
- 1 - move backward.
- 2 - turn left.
- 3 - turn right.

### Solving condition
The task is episodic, and to solve the environment, agent must score an average of +13 out of 100 consecutive plots.

## Algrithm
This project implement a Value Based method called Deep Q-Networks. Refer the paper [Human-level control through deep reinforcement learning](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf) to see more Deep Q-Networks algrithm details. And refer [the Report file](https://github.com/oliver1112/udacity-DRL-nanodegree-project-Navigation/blob/master/report.md) to see my hyperparameters details, along with ideas for future work.

you can see from the below gif that the trained agent learn how to navigate to get yellow bananas while avoiding blue ones.
![Train][gif1]

## Dependencies
To set up your python environment to run the code in this repository, follow the instructions below.


1. please follow the instructions in the python file to set up your Python environment. By following these instructions, you will install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project.
```bash
pip install .
```


2. I use the Windows (64-bit) operating system, [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip) to install the banana game environment. And unzip (or decompress) the file in the folder.
For other operating system, please download the environment from one of the links below.
- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)


3. Follow the instructions in `Navigation.ipynb` to see my code!  

