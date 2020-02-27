[//]: # (Image References)
[image3]: https://github.com/oliver1112/udacity-DRL-nanodegree-project-Navigation/blob/master/assets/DQN.png "Plot"
[image2]: https://github.com/oliver1112/udacity-DRL-nanodegree-project-Navigation/blob/master/assets/DQN%20Pseudocode.png "Pseudocode"

# Project Report
## Learning Algorithm and hyperparameters
In the DQN algorithm, a 4 layers neural network is used to approximate the value function, with the parameters of state space dimension 
37 to inputs layer, action space dimension 4 to the output layer and 64 to the middle hidden layers. A relu function is used after each 
hidden layers to improve the approximate ability of the netword. The neural network is created with Pytorch frame. Adam optimizer 
is used and the learning rate is set LR = 0.0005 


The epsilon greedy policy is used to balance the Exploration-Exploitation Dilemma. With hyperparameters epsilon decrease from 1 to 0.01 with exponential decline factor 0.99
- Experience Replay


To fully utilize the state-action pairs, experience replay is used to steep up the learning process. The replay buffer size is set to 100000
and the batch size is set to 64

- Target Network


To decrease oscillation phenomenon, A target network is used to speed up the convergence process. The target network is softly updated 
every 4 episode with hyperparameter tau = 0.001 

### Pseudocode
![Pseudocode][image2]
This algorithm screenshot is taken from the [Deep Reinforcement Learning Nanodegree course](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893)



## Plot of Rewards
The Environment solved in 300 episodes. The reward changes with the number of episodes as shown below:
![Plot][image3]




## Ideas for Future Work
- Trying to implement a double DQN, a dueling DQN, or prioritized experience replay.
- Trying to solve the problem direatly from pixels without the ray-based state space. A convolutional neural network would be used at the input of the network in order to process the raw pixels.
