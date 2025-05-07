## 🐦 Flappy Bird AI using NEAT
An AI agent that learns to play Flappy Bird using the **NEAT (NeuroEvolution of Augmenting Topologies)** algorithm. This project uses [Pygame](https://www.pygame.org/) for game rendering and [NEAT-Python](https://neat-python.readthedocs.io/en/latest/) for training the neural networks. The agent evolves over generations, improving its ability to navigate pipes without human intervention.

## 🚀 Features

- 🧠 AI-controlled bird using NEAT
- 🏞️ Real-time graphics using Pygame
- 📈 Generation tracking and scoring
- 💾 Configurable NEAT parameters
- 🔄 Replayable and reproducible simulations

<img src="fp.gif" width="450" height="450">

## 🧰 Technologies Used

- **Python 3.x**
- **Pygame** – for rendering and game mechanics
- **NEAT-Python** – for neuroevolution and fitness evaluation

## How NEAT Works in This Project

- Each bird is controlled by a neural network.
- Networks are evolved using NEAT over multiple generations.
- Fitness is based on survival time and number of pipes passed.
- The best-performing networks survive and mutate to improve over time.

### Each bird is controlled by a neural network that receives **3 inputs**:

- 🐤 Bird’s vertical position
- 📏 Distance to the next pipe (top)
- 📏 Distance to the next pipe (bottom)

The **single output** decides:  
➡️ `Jump` if the value > 0.5  
➡️ `Do nothing` otherwise

Fitness increases with time survived, and decreases for collisions or bad jumps.

## 🛠️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Tynoee/AI-Flappy-Bird-Game.git
cd flappy-bird-ai



