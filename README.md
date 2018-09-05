
# DRLND Navigation

The purpose of this project is to an agent to navigate (and collect bananas!) in a large, square world.

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Environment"

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

**0** - move forward.
**1** - move backward.
**2** - turn left.
**3** - turn right.

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

 ## Getting Started
 
 ### Virtual environment
 
To install the dependencies follow the instructions bellow:

1 - Create (and activate) a new environment with Python 3.6.

- Linux or Mac:
```
conda create --name drlnd python=3.6 
source activate drlnd
```
- Windows:
```
conda create --name drlnd python=3.6 
activate drlnd
```

2 - Go to the python folder and install the dependencies on your virtual environment:

```
cd python
pip install .
```

3 - (Optional) If you would like to run the code on the notebook you need to create an IPython kernel for this virtual environment:

```
python -m ipykernel install --user --name drlnd --display-name "drlnd"
```
 
 ### Unity Environment
 
To run the environment you will need to:

1 - Download the unity files from here:

- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

2 - Place the file in the p1_navigation/ folder in the DRLND GitHub repository, and unzip (or decompress) the file.

## Instructions

Now you are ready to train an agent and watch it perform the task.

### Training

To train an agent simply run:

```
python train_agent.py
```

And you should see the score of each episode on the terminal. When the agent reaches the desired score of 13.0 the training finishes and the weights of the network of the agent is saved on **checkpoint.pth**.

### Watch the trained agent

After training the agent, with the checkpoint file in the repository folder, run:

```
python test_agent.py
```