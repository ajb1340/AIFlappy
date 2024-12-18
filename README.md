Flappy Bird NEAT AI
This project implements a Flappy Bird clone powered by a NeuroEvolution of Augmenting Topologies (NEAT) algorithm. The goal is to train an AI to play Flappy Bird autonomously by evolving neural networks over successive generations.

Features
  Dynamic Gameplay: The game includes obstacles (pipes), a scrolling background, and an animated bird character with smooth physics.
  NEAT Integration: Uses the NEAT-Python library to train a population of neural networks.
  Real-time Visualization: Displays the current generation, score, and the birds as they learn to navigate pipes.
  Fitness Evaluation: Encourages smarter birds by assigning fitness based on survival time and passing pipes.
How It Works
  Bird Physics: Each bird has realistic physics including jump velocity, gravity, and rotation.
  Pipe System: Pipes are randomly generated with gaps that adjust difficulty as the AI improves.
  Neural Network Input: Each bird's neural network receives the following inputs:
  Vertical distance from the bird to the top of the pipe gap.
  Vertical distance from the bird to the bottom of the pipe gap.
  Current bird height.
  Neuroevolution: The NEAT algorithm evolves the population by:
  Increasing fitness for survival and successful pipe navigation.
  Penalizing collisions and out-of-bound movements.

Configuration
The NEAT algorithm is configured through a NEAT_Config.txt file
. You can adjust parameters such as population size, mutation rates, and fitness thresholds to experiment with different learning behaviors.
