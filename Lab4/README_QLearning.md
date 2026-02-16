# Q-learning on CartPole environment
## Lab session

In this lab session we will tackle the Q-Learning algorithm on a system in which the state space is continuous: The [CartPole](https://gymnasium.farama.org/environments/classic_control/cart_pole) environment.

The Cartpole problem is theoretically a rather simple problem, which can be solved by calculating the physics of the problem, but an RL-agent does not have that prior knowledge.


This lab will build upon the concepts introduced in the lecture and help you apply your knowledge to a simple problem.

### Educational Objectives

* Know how to apply Q-learning algorithm in a new problem.
* Use discretization to be able to apply tabular Q-learning to a system with continuous state space.

### Getting Started

Please group up in pairs and open the corresponding notebook. It contains the instructions of the task.

### Tasks

This lab is designed for you to be able to apply the Q-Learning method in a new environment.
Read the explanations in the notebook, let the code run and observe the resulting plot.
Then, do the following tasks:

* **Where is the Q-Learning algorithm?**:
    Find out where the training is happening.
    Implement the functions to update the Q-value. Can you use the same expressions you used for the Gridworld environment?
    What is the actual value of the learning rate? How does it change.

* **Extend the plotting**:
    Implement a function to plot both the learning rate and the epsilon over the course of the training.

* **Discretization**:
    Change the number of buckets used for discretization. What is the effect on learning?


* **Initial conditions**:
    Adapt the code to run the training process 10 times with different seends of the random number generator. Does the learning process and outcome change across runs?


* **Update the code**:
    Update the code to use a fixed learning rate to 0.1 and retrain. How does the learning changes compared with the initial implementation?
    Now, do the same with the *epsilon* parameter.



### Key Takeaways

* **Q-Learning**:
    Q-Learning is a powerful model-free reinforcement learning algorithm that helps agents learn the values of state-action pairs to make optimal decisions.
* **Building on Foundations**:
    Q-Learning builds on the foundational concepts of MDPs, Monte Carlo algorithms, Dynamic programming, and Time-Differences.
    * Monte Carlo learns from entire trajectories.
    * Dynamic Programming learns from looking one step ahead on all actions
    * Q-Learning looks one step ahead on one action.
* **Value Functions and Action-Value Functions**:
    Q-Learning is an action-value based approach that helps agents learn the action-value function (Q) to make informed decisions.
* **Experiment and Iterate**:
    The best way to grasp the nuances of Q-Learning is through experimentation.
    Try different scenarios, hyperparameters, and modifications to gain a deeper understanding.


## RL examples

* Robotics: Google DeepMind used Q-Learning to teach virtual humans and creatures to move over obstacles in 2017 ([video](https://www.youtube.com/watch?v=hx_bgoTF7bs), [publication](https://www.deepmind.com/publications/emergence-of-locomotion-behaviours-in-rich-environments))
* QT-Opt: Google AI used a variant of deep Q-Learning to teach robots to grasp objects, with 96% successful grasp attempts in 2018 ([video](https://www.youtube.com/watch?v=W4joe3zzglU), [preprint](https://arxiv.org/abs/1806.10293)).
* TD-Gammon: Using Temporal Difference Learning, TD-Gammon almost rivaled the top human backgammon players in 1992, with the latest version making significantly less errors than the top backgammon player Malcolm Davis in 1998.
* Deep Q-Network (DQN): DeepMind trained DQN to play Atari games, beating competitive RL agents and even human players by a landslide in 2013 ([paper](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf)). We'll cover these type of networks later this semester.
