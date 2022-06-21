 # Introduction of repositories
 A few years back OpenAI released the “baselines” repository which included implementations of most of the major deep reinforcement learning algorithms.
 - stable baslines
 This repository was turned into the Stable Baselines library intended for beginners and practitioners of reinforcement learning to easily use to learn Gym environments. 
 - CnnPolicy
 The CnnPolicy in it is just a deep convolutional neural network object that Stable Baselines includes which automatically resizes the input and output layers of the neural network to adapt to the observation and action space of the environment. 
 - supersuit
 SuperSuit is a package that provides preprocessing functions for both Gym and PettingZoo environments, as we’ll see below. Environments and wrappers are versioned to ensure comparisons are precisely reproducible in academic research.
 github for supersuit: https://github.com/Farama-Foundation/SuperSuit

# introduction of Multiagent
In general it’s the same as single agent reinforcement learning, where each agent is trying to learn it’s own policy to optimize its own reward.
Using a central policy for all agents is possible, but multiple agents would have to communicate with a central server to compute their actions (which is problematic in most real world scenarios), so in practice decentralized multi-agent reinforcement learning is used.
 

# installing PettingZoo: https://github.com/Farama-Foundation/PettingZoo
# create venv
python3 -m venv marl-env
# active venv
source marl-env/bin/activate
# upgrade really old pip version on my system
pip install --upgrade pip
# install packages
pip install pettingzoo[classic]
pip install spyder-notebook
pip install dill

