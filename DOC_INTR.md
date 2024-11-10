# MASAC vs ISAC
## Project assumtions
TBD - rysio
## Project environmment
### Software
#### BenchMARL: Multi-Agent Reinforcement Learning Library
BenchMARL is Multi-Agent Reinforcement Learning (MARL) library focused on standardized benchmarking across a variety of algorithms and environments. Its mission is to present a standardized interface that allows easy integration of new algorithms and environments to provide a fair comparison with existing solutions. Core design principles include:

- **Reproducibility**: Achieved through systematic grounding and standardization of configuration.
- **Standardized Reporting**: Strong plotting and reporting.
- **Modular Experimentation**: Experiments that are independent of the algorithm, environment, and model choices.
- **Broad MARL Ecosystem Coverage**: Breadth over the MARL ecosystem.
- **Ease of Integration**: Easy implementation of new algorithms, environments, and models.
- **TorchRL Integration**: Leveraging the know-how and infrastructure of TorchRL, without reinventing the wheel.

#### MeltingPot
Melting Pot evaluates how well agents generalize to new social environments, including interactions with both known and unfamiliar individuals. It was designed to test a broad range of social interactions including cooperation, competition, reciprocation, stubbornness and trust. Melting Pot offers researchers a set of over 50 multi-agent reinforcement learning substrates (multi-agent games) and over 256 unique test scenarios for evaluation. The performance of agents on test scenarios allows to assess agents in:

- **Adaptability**: Perform well across a range of social situations where individuals are interdependent.
- **Interpersonal Generalization**: Interact effectively with unfamiliar individuals not seen during training.

### Technical realisation
Python scripts for experiments and Notebooks for visualisation
rysio
## Algorithms to be implemented and tested
### ISAC
rysio
### MASAC: Multi Agent adaptation of Soft Actor Critic Reinforcement Learning Algorithm
MASAC is an extension of the Soft Actor-Critic (SAC) reinforcement learning algorithm, adapted for multi-agent environments. SAC is a popular model-free, off-policy algorithm that combines elements of both maximum entropy reinforcement learning and Q-learning, aiming to achieve both stability and high exploration. MASAC builds on this approach by allowing multiple agents to learn simultaneously in a shared environment, where each agent optimizes its own policy while considering interactions with other agents.
## Necessary libraries
tbd
## Experiment propositions
### Collaborative Cooking - Cooperative
In this scenario, agents work together in a kitchen setting to prepare and serve food items. They must coordinate their actions to complete tasks efficiently, such as gathering ingredients, cooking, and serving dishes within a time limit. Success depends on effective teamwork and sharing resources. This environment encourages agents to optimize collective outcomes, making it an example of a cooperative problem
### Chicken in the matrix: Arena - Competitive
Individuals can gather resources of different colors. Players’ encounters are resolved with thesame payout matrix as the game ’Chicken’, in which both players attempting to take advantage of the other leads to the worst outcome for both. Collecting red resources pushes one’s strategy choice toward playing ‘hawk‘ while collecting green resources pushes it toward playing ‘dove‘.
### Allelopathic Harvest - Mixed (Primarily Cooperative with Competitive Elements)
Clean Up is a seven player game. Players are rewarded for collecting apples (reward +1). In Clean Up, apples grow in an orchard at a rate inversely related to the cleanliness of a nearby river. The river accumulates pollution at a constant rate. Beyond a certain threshold of pollution, the apple growth rate in the orchard drops to zero. Players have an additional action allowing them to clean a small amount of pollution from the river. However, the cleaning action only works on pollution within a small distance in front of the agents, requiring them to physically leave the apple or chard to clean the river. Thus, players maintain a public good of orchard regrowth through effortful contributions. Players are also able to zap others with a beam that removes any player hit from the game for 50 steps.
