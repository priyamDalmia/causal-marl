# Causal Multi Agent Reinforcement Learning with RlLib.

This repository contains implementations of multi-agent reinforcement learning algorithms and some causality modules, on the new [RlLib]() API.  

<!-- Shields
1. python versions 
2. ray versions 
3. tests passing 
4. build passing
5. code coverage  
 -->

[![build](https://github.com/priyamDalmia/my-py-package/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/priyamDalmia/my-py-package/actions/workflows/build.yml)

![Ray Version](https://img.shields.io/badge/Ray-2.30.0%2B-blue)

![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)

![PyPI Version](https://img.shields.io/pypi/v/your-package-name)

![GitHub Release](https://img.shields.io/github/v/release/your-username/your-repo)

![GitHub Tag](https://img.shields.io/github/v/tag/your-username/your-repo)

# Overview 

## Algorithms

<!-- A table the list the algorithms that have been completed and benchmarked.  -->

1. Independent Learners 

2. Centralized Critic

3. Communication and Control

4. Hierarchial Multi Agent Systems 

## Project Structure and Usage

The project structure here mimics the one at [rllib]() for consistency. Algorithms and Modules can be imported and extended using the same principles of the rllib library. 


```python
from causal_marl.algorithms.qmix import QMIXConfig
from rllib.algorithms.ppo import PPO

algo_config = QMIXConfig()
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

Since this libary relies on the Ray and Rllib framework, I would recommened running an optional test to see if everything is correctly installed.

# Contributing 

## Creating a new algorithm

# License

# Citation 