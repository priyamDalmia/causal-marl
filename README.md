# Causal Multi Agent Reinforcement Learning with RlLib.

This repository contains implementations of multi-agent reinforcement learning algorithms and intrinsic causality modules, built on the new [RlLib]() API.  

[![build](https://github.com/priyamDalmia/my-py-package/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/priyamDalmia/my-py-package/actions/workflows/build.yml)
![Ray Version](https://img.shields.io/badge/Ray-2.30.0%2B-blue)
![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)
![PyPI Version](https://img.shields.io/pypi/v/your-package-name)
<!-- 
![GitHub Release](https://img.shields.io/github/v/release/your-username/your-repo)

![GitHub Tag](https://img.shields.io/github/v/tag/your-username/your-repo) -->

# Overview 

Multi-agent reinforcement learning (MARL) is an extension of reinforcement learning (RL) where multiple agents interact within the same environment. Each agent learns and adapts its strategy based on its own experiences and observations, while also (or not) considering the actions of other agents. 

The RLlib library, built upon the Ray distributed compute framework, provides a set of tools and utilities that makes testing and training reinforcement learning algorithms easy. It takes care of common design patterns, ubiquitous to many modern RL algorithms, and helps the user focus only on the important bits. 

Multi agent RL often extends single agent RL but adding only a few new component on top of the original architecture. This library contains a few such components to derive a series of popular multi agent reinforcement learning algorithms. 

## Algorithms

<!-- A table the list the algorithms that have been completed and benchmarked.  -->

1. Independent Learners 

2. Centralized Critic
    - COMA 
    - QMIX 
    - MADDPG 

3. Communication and Control
    - RIAL 
    - CommNet
    - Causal Comm 

4. Hierarchial Multi Agent Systems 
    - Feudal (limited)
    - Feudal General

## Project Structure and Usage

The project structure here mimics the one at [rllib]() for consistency and interoperability. Algorithms and Modules (and connectors) can be imported and extended using the same format of the rllib library. 


```python
from causal_marl.algorithms.rial import RIALConfig 
from rllib.algorithms.ppo import PPO

algo_config = RIALConfig()
                .learner(PPO)
```

## Installation

```bash
# activate your virtual environment
source .venv/bin/activate 
# install the package
pip install causal_marl
```

### Optional 

Since this library relies on the Ray and Rllib framework, I would recommend running an optional test to see if everything is correctly installed.

# Contributing 

## Creating a new algorithm

Follow the guide at Rllib if you want to create a new algorithm from scratch. If you only want to tweak from multi agent agents, follow this guide that explains how I've built these algorithms. 

# Citation 

Citation coming soon!