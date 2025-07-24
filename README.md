# Real-Coded Genetic Algorithm (RGA) Process
This RGA implementation optimizes user-defined or standard objective functions using the pymoo framework. It supports mixed-variable optimization (continuous, discrete, binary) with constraints.

# Process Overview:
Initialization: Loads parameters (variables, bounds, population size, constraints) from user_def.txt or user input.

Population Setup: Initializes the population using custom sampling tailored to variable types.

Evaluation: Calculates fitness using dynamically loaded objective functions.

Evolution Loop (for ngen generations):

 1.Selection: Chooses parents using tournament selection.

 2.Crossover: Applies real-coded crossover to generate offspring.

 3.Mutation: Applies mutation with customized logic for mixed types.

 4.Survivor Selection:

   1.Elite Preservation: Best nelite individuals are retained.

   2.Worst Replacement: Low-performing individuals are replaced to enhance diversity and convergence.

Constraint Handling: Ensures feasible solutions using validation logic.

Reporting: Outputs reports per generation or per run, along with convergence plots.

This modular and configurable RGA structure ensures flexible and robust optimization for complex, constrained problems.
