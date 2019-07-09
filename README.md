# DQN_and_extensions
A sandbox for exploring basic Deep RL algorithms.

This repository is an exploration of basic deep RL algorithms. DQN and simple extensions will be used to solve various OpenAI gym enviornments and Unity ML-agents environments.

#### First application: Unity Banana environment.

The goal of the agent is to collect yellow bananas (rewarded +1) and avoid blue bananas (rewarded -1), by using simple navigation actions (4 actions available, forward, backward, turn left, turn right). The state space is described through a 37-dimensional vector that contains a description of the agent location, speed and a ray-based representation of the current objects in the envorment. 

The envorment is solved when the agent acheives a score of 13 or more averaged over 100 consequtive episodes. 

To run the enviornment locally a few required packages are necessary.

1) Udacity provides [this github repository](https://github.com/udacity/deep-reinforcement-learning#dependencies) with many of the dependencies required to run the environment. Follow the instructions in the readme.md file under thea heading 'dependencies' to clone a copy and install the required packages. 
     * Note that openAI minimal install gym already includes box2d and classic control librarys, so those steps are no longer needed. (can be installed through: pip install box2d, if needed)
     * Also note that the instructions create a conda environment 'drlnd' and it is important to ensure this envornment is active as you proceed.
     * Note also that it will be required to install ipykernel (pip install ipykernel) to execute all the steps.

2) Installing Unity enviroments is an option, but it will be easier to download only the required executable provided by Udacity. [The Windows 64bit compabtible version](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip) is included here for reference, but other versions can be found on the Udacity github repository.

3) For hyperparameters optimization, I used the package 'bayesian-optimization', which can be installed by running
    pip install bayesian-optimization

4) To run the enviroment locally additional Unity packages are required as detailed [here](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation-Windows.md). 
    * **Note:** it is also important to run 'pip install unityagents' which is not mentioned in the instructions.
    
In the jupyter notebook *'Navigation.ipynb'*, the agent is trained and tested on a simplified ray-based state description.




