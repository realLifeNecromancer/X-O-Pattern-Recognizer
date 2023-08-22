# X-O-Pattern-Recognizer

# X and O Neural Network

This repository contains an implementation of a simple neural network designed to differentiate between the letters X and O based on user inputs on a 5x5 panel. The neural network utilizes the Hebbian learning algorithm to learn and recognize the patterns of X and O.

## Overview

The neural network is implemented using Python and consists of two main components:

1. `neuralNetworks.ipynb`: This Jupyter Notebook contains the core logic of the neural network and the Hebbian learning algorithm. It provides the implementation for the training process, including weight and bias adjustments, and activation functions. The notebook initializes the weights and bias and contains the code for the Hebbian learning algorithm.

2. `Perdict.ipynb`: This Jupyter Notebook implements the graphical user interface (GUI) using the Tkinter library. The GUI allows users to interact with a 5x5 panel of buttons to create patterns of X and O. These patterns are then passed to the trained neural network for prediction. The GUI also includes options to reset the panel and make predictions.

## Getting Started

To use this codebase, follow these steps:

1. Clone this repository to your local machine using Git.

   ```bash
   git clone https://github.com/realLifeNecromancer/X-O-Pattern-Recognizer.git
   ```

2. Install the required dependencies by running the following command:

   ```bash
   pip install numpy tk
   ```

3. Open and run the `Perdict.ipynb` Jupyter Notebook using a Jupyter Notebook environment.

4. Follow the instructions in the notebook to interact with the GUI. You can click on the buttons in the 5x5 panel to create patterns of X and O. After creating a pattern, click the "Predict" button to let the neural network make a prediction.

## Requirements

- Python (3.x recommended)
- Jupyter Notebook
- NumPy library
- Tkinter library

## Files and Functionality

- `neuralNetworks.ipynb`: This notebook contains the following functions and components:
  - `step_function`: The activation function used for output calculation.
  - `calculate_output`: Computes the output of the neural network based on the input instance, weights, and bias.
  - `hebb`: Implements the Hebbian learning algorithm to train the neural network. It initializes weights and bias and updates them based on the training data.
  
- `Perdict.ipynb`: This notebook provides the graphical user interface for interaction with the neural network:
  - Buttons in a 5x5 grid: Users can click the buttons to create patterns of X and O.
  - `click` function: Handles button clicks, toggling between -1 and 1 values for buttons.
  - `perdict` function: Sends the created pattern to the trained neural network and displays whether the pattern represents an X or an O.
  - `reset_the_buttons` function: Resets all buttons to their initial state.
  
## License

This project is licensed under the [MIT License](LICENSE).
