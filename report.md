[//]: # (Image References)


# Project Report
## Learning Algorithm and hyperparameters
In the DQN algorithm, a 4 layers neural network is used to approximate the value function, with the parameters of state space dimension 
37 to inputs layer, action space dimension 4 to the output layer and 64 to the middle hidden layers. A relu function is used after each 
hidden layers to improve the approximate ability of the netword. The neural network is created with Pytorch frame. Adam optimizer 
is used and the learning rate is set LR = 0.0005 


To fully utilize the state-action pairs, experience replay is used to steep up the learning process. The replay buffer size is set to 100000
and the batch size is set to 64


To decrease oscillation phenomenon, A target network is used to speed up the convergence process. The target network is softly updated 
every 4 episode with hyperparameter \tau = 0.001 


The epsilon greedy policy is used to balance the Exploration-Exploitation Dilemma. With hyperparameters \epsilon_0 = 1 and exponential 
decline factor eps_decay=0.99 until the final \epsilon_t = 0.01


## Plot of Rewards
The Environment solved in 300 episodes,	get an Average Score: 13.05
![Trained Agent][image3]




## Ideas for Future Work
