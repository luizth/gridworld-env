# gridworld-env

Gridworld environments in reinforcement learning.

## Installation

You can download and make the library available in your project using _pip_.

```bash
$ pip install git+https://github.com/luizth/gridworld-env.git
```

## Usage

Simple instructions on how to import and instanciate an environment using available configurations.

```python
from gridworld_env.gridworld import GridWorld
from gridworld_env.room_design import available_configs

print(available_configs)  # dict_keys(['two_rooms_penalty_v0', 'four_rooms_penalty_v0'])

env = GridWorld(available_configs.sample())
env_tworooms = GridWorld(available_configs.get('two_rooms_penalty_v0'))
```

## Reference

The Gridworld Domain is canonical in reinforcement learning research.

This implementation was adapted from code from STOMP open repository (https://github.com/ramos-ai/STOMP), from Arturo de Souza.
