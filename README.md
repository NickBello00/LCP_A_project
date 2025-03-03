Conway's Game of Life is a foundational cellular automaton devised by mathematician John Horton Conway in 1970. It simulates emergent complexity through simple rules governing cell birth, survival, and death on a 2D grid, with no player input required after initialization
It is designed to model the evolution of a grid of cells over time, following simple rules for cell birth, survival, and death. The program includes features for initializing the grid with various patterns, evolving the system through time steps, and analyzing the evolution of the system.

KEY COMPONENTS
-> Initialization:

The program can initialize the grid with random configurations or specific patterns fetched from ConwayLife.com, such as "glider," "pulsar," or "gosperglidergun."

The initial_state function handles pattern retrieval and grid setup.

-> EVOLUTION:

The NextStep function applies the Game of Life rules to evolve the grid from one generation to the next.

The evolve function runs the simulation for a specified number of generations and can display the grid at each step.

-> ANALYSIS:

The analyze_base_game_of_life function analyzes the simulation's history, plotting the number of live cells over time and the mean square distance of live cells from their center of mass.

It also detects periodicity in the system's evolution.

-> VISUALIZATION:

The program uses matplotlib to visualize the grid at each generation, with options to display the initial and final states.

The PlotGrid function handles visualization, including grid layout and cell representation.

TECHNICAL DETAILS:

-> Libraries Used: NumPy for numerical operations, SciPy for convolution (neighbor counting), matplotlib for visualization, and requests for fetching patterns from the web.

-> Data Structures: 2D NumPy arrays represent the grid, with 0s for dead cells and 1s for live cells.

-> Rules Application: The Game of Life rules are applied using a convolution filter to count neighbors efficiently.

Example Use Cases
Random Initialization: Run a simulation with a random initial configuration to observe emergent patterns.

Pattern Analysis: Initialize with a specific pattern (e.g., "glider") and analyze its behavior over time.

Periodicity Detection: Use the find_periodicity function to identify repeating patterns in the system's evolution.
