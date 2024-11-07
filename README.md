# Deep_Learning_Applications
Project for Deep Learning Applications - instructor: Dr. Pozzi

# HalfCheetah-v3 Reinforcement Learning

This repository contains two Jupyter notebooks demonstrating different approaches to reinforcement learning on the HalfCheetah-v3 environment from OpenAI Gym.

## Usage

To run the notebooks is recommended the Google Colab environment, this because many package are linux native and we have the guarantee of accellerator support.

## Notebooks

1. `A2C_HalfCheetah.ipynb`: Implementation of the Advantage Actor-Critic (A2C) algorithm.
2. `DecisionTransformer_HalfCheetah.ipynb`: Offline reinforcement learning using a Decision Transformer model.

Notebooks are uploaded inside their respective folders alongside trained agents, checkpoints and recorded videos.

## Environment

Both notebooks use the HalfCheetah-v3 environment from OpenAI Gym. This environment simulates a 2D cheetah robot and aims to make it run as fast as possible.

## Algorithms

### A2C (Advantage Actor-Critic)

The A2C algorithm is an on-policy reinforcement learning method that combines:
- An actor that decides which action to take
- A critic that estimates the value function

This notebook demonstrates the training process and results of applying A2C to the HalfCheetah-v3 environment.

### Decision Transformer

The Decision Transformer is a novel approach to reinforcement learning that frames the problem as a sequence modeling task. This notebook shows how to use a Decision Transformer in an offline setting, learning from pre-collected data without direct interaction with the environment.

## Requirements

Detailed requirements can be found in the `requirements.txt` file.


## Results

From results we can see a positive, but not enough good performance, of the A2C algorithm model. 
 * Average performance: Mean reward = 1297.53 +/- 342.18
 * Baseline performance: The HalfCheetah-v3 environment is considered solved when achieving an average reward of 4800 over 100 consecutive episodes.
Better performances could be maybe achieved by employing more advanced algorithms like PPO, SAC, or TD3.

From what concern Decision Transformer model we get a better performance but it must be considered that this kind of approach has been implemented in an offline way, and a more solid comparison could arise by implementing an online approach, and this could be definetely a further step.


## Contributing

Migliori Luca - luca.migliori01@icatt.it
