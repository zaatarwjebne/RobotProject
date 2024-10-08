# RobotProject

Introducing **BOB**, a robot designed to compete in the **COGS 300 class competition**. The project utilizes **ML-Agents**, an AI toolkit for the Unity game engine, to program BOB to compete in a 2-minute game.

## Project Overview

In this project, BOB competes against other robots with the goal of collecting and securing green balls within a time limit. Our robot uses machine learning techniques to strategize its gameplay, making it a powerful competitor in the class competition.

## Gameplay

- **Objective**: Each robot starts on opposite ends of the arena with green balls in the center. The goal is to collect as many green balls as possible and bring them back to the robot’s starting area.
- **Mechanics**:
  - BOB can grab and steal balls from opponents.
  - BOB can shoot lasers at opponents to slow them down.

## Technical Details

The core functionality of BOB is implemented in C# using the **Unity** game engine, and its behavior is controlled by machine learning algorithms via **ML-Agents**.

Our code is mainly found in:

- **ML-Agents**: Used for training BOB's behavior through reinforcement learning.
- **C# Scripts**: The code controlling BOB is located in `Assets/Resources/BOB`.


### Key Files

- `BOB.cs`: Contains the logic for BOB's actions and interactions in the game.
- `bobnn10.onnx`: The trained neural network model used by BOB during gameplay.
- `AgentTraining.unity`: The training environment for BOB where it learns to optimize its behavior.

## How to Run the Project

1. Clone the repository:
    ```bash
    git clone https://github.com/zaatarwjebne/RobotProject.git
    ```
2. Open the project in **Unity**.
3. Ensure **ML-Agents** is set up in your Unity environment. You can follow the [ML-Agents documentation](https://github.com/Unity-Technologies/ml-agents) for setup instructions.
4. Run the scenes:
    - Use `AgentTraining.unity` to observe the training process.
    - Run `AgentTesting.unity` to see BOB in action.

## Results

BOB was tested in multiple environments and ranked **5th** in the **COGS 300 class competition**. Its ability to quickly learn and adapt during gameplay allowed it to compete at a high level.

### Results Folder

- The `results/run1` directory contains results data 
## Technologies Used

- **Unity**: For building the game environment and robot behaviors.
- **ML-Agents**: Used for machine learning and reinforcement learning.
- **C#**: The primary programming language for scripting the robot’s behavior.
- **ONNX**: For using pre-trained neural network models with ML-Agents.

## Future Improvements

- Refine BOB's ball collection strategy using advanced reinforcement learning techniques.
- Improve its laser shooting accuracy and defensive mechanisms.
- Implement multi-agent cooperation for more complex team-based games.

