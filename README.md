# Multi-Armed Bandit Simulation

This Jupyter notebook implements a simulation of the multi-armed bandit problem using a stochastic approach. It provides a framework for creating and running bandit simulations, which can be useful for studying reinforcement learning algorithms and decision-making under uncertainty.

## Features

- Implements Bernoulli bandits with random probability distributions
- Simulates multi-armed bandit games with a configurable number of bandits and time steps
- Provides a function to run multiple simulations and average the results
- Includes example usage for both a single game and a full simulation

## Requirements

- Python 3.x
- Jupyter Notebook or JupyterLab
- NumPy

## Installation

1. Ensure you have Python 3.x installed on your system.
2. Install Jupyter Notebook if you haven't already:
   ```
   pip install jupyter
   ```
3. Install NumPy if you haven't already:
   ```
   pip install numpy
   ```
4. Download the `Multi_Armed_Bandit_Simulation.ipynb` file to your local machine.

## Usage

### Running the Notebook

1. Navigate to the directory containing the notebook in your terminal or command prompt.
2. Start Jupyter Notebook:
   ```
   jupyter notebook
   ```
3. In the Jupyter interface that opens in your web browser, click on `Multi_Armed_Bandit_Simulation.ipynb` to open it.
4. You can run individual cells by selecting them and pressing Shift+Enter, or run all cells from the "Cell" menu by selecting "Run All".

### Customizing the Simulation

To customize the simulation parameters, modify the values in the cells containing the example usage. For instance:

```python
# Run a simple game
game = BanditsGame(K=5, T=50)  # 5 bandits, 50 time steps
game.run_stochastic()

# Run the full simulation
stochastic_results = run_simulation(n_runs=20, runs_per_game=200, K=5, T=2000)
```

### Using in Your Own Projects

You can copy the relevant cells containing the classes and functions from this notebook to use in your own Jupyter notebooks or Python scripts.

## Notebook Structure

The notebook is structured as follows:

1. Introduction and imports
2. `BernoulliBandit` class definition
3. `BanditsGame` class definition
4. `run_simulation` function definition
5. Example of running a simple game
6. Example of running a full simulation
7. Results analysis and visualization (if applicable)

## Extending the Code

You can extend this simulation by:

1. Implementing different types of bandits (e.g., Gaussian bandits)
2. Adding new bandit selection strategies (e.g., epsilon-greedy, UCB)
3. Implementing visualization of the results
4. Adding more complex reward structures

## Contributing

Feel free to fork this project, submit pull requests, or suggest improvements by opening an issue in the project repository.

## License

This project is open-source and available under the MIT License.
