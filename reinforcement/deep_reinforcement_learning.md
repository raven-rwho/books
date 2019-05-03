# Deep Reinforcement Learning Hands-On - Maxim lapan

## Chapter 1 - What is reinforcement Learning?
RL is a third category of ML methods. It lays in the middle of supervised and unsupervised methods. By "palying" an environment and monitoring the given reward, which is often defined through a ploicy - it is able to generate the "labeled data" itself.
As chapter 4 shows with an catpole envorinment - by feeding a neural network with the observations of "winning" episodes - RL is able to play cartpole without any implementaion/explanation of the environment!

### Reward

### Agent

### Environment

### Actions

### Observations

## Chapter 2 - OpenAI Gym
[Gym](https://www.openai.com) is a framework that implements all necessary parts of RL-Learning (see above). It provides hundreds of already prepared environments - from borad games over algorithmic challenges to parameter tuning and doom. 

## Chapter 3 - Deep Learning with PyTorch
Deep Learning Libraries can be discriminated into two categories:
 * **static graph** - the graph of the NN needs to be compeletedly defined before the calculation. This offers advantages for the library to optimize the calculation - means it is often faster - but it limits the possibilities to work with the network. Tensorflow is using this method.
 * **dynamic graph** - it is not necessary to define the graph in advance exactly. This allows the freedom to perform any tranformations on the actual data. This is also called ** notebook gradients **. PyTorch implements this method.

### TensorBoard 
Nice web based framework to monitor the progress of the NN training. Via [OSS](https://github.com/lanpa/tensorboard-pytorch) libraries also usable for PyTorch.
### Example
**GAN on Atari images** - The chapter results in an example which implements an generative adversarial network which __generates__ Atari images and on the other hand __dicriminates__ if this images are fake or real.
## Chapter 4 - The Cross-Entropy Method
1. Play N-Numbers of epsodes.
2. Calculate the total reward of ewach episode.
3. Chooce the episodes with the highest reward (> the some percentile)
4. Train on the winning episodes
5. Repeat from step one.

__Limitations of cross entropy - shown with the noisy frozenlake environment__ 
* the training episodes have to be finite
* the total reward need to have enough variability
* no intermediate indication if the agent has succeeded or failed

## Chapter 5 - Tabular Learning and the Bellman Equation


