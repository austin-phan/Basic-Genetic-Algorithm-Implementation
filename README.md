# Basic-Genetic-Algorithm-Implementation
 A basic genetic algorithm implementation intended as a baseline design for a larger project.

# Components of a Genetic Algorithm

 Population
 - Set of candidate solutions, also called individuals
 - Represented as a "chromosome" which can be coded as, binary strings, arrays, or other data structures
 - In this implementation, each chromosome represents a set of input values

 Fitness Function
 - Evalutes each individual's ability to solve the problem
 - In certain implementations, 0 may be used as a solved solution, but generally higher scores are better
 Selection Function
 - Chooses individuals to reproduce based on their fitness score
 - Roulette wheel selection are based on a probability proportional to their fitness
 - Tournament selection is where a subset is chosen at random and the fittest individual is chosen from this subset
 - Rank-based selecrtion ranks based on their fitness, selection probability is assigned based on these ranks rather than raw fitness values

 Crossover function
 - Combines infromation from two individuals to create offspring
 - Aims to inhereit useful traits from the parents
 - Single-point cross over chooses a random point and swaps genetic material at that point
 - Multi-point uses multiple of these random points for more complex genetic combinations
 - Uniform crossover randomly decides for all the genes

 Mutation function
 - Introduces random changes to assist diversity

# The General Genetic Algorithmic Process
 
 Step 1: Initialization
 - Generate an initial population of random inidivuals
 - Create a diverse set

 Step 2: Evaluation
 - Calculate the fitness of each individual
 - Use the fitness function to evaluate the viability of each solution

 Step 3: Selection
 - Using the selection criteria, select based on fitness
 - Determines the parents

 Step 4: Crossover
 - Generate new solutions using the parents

 Step 5: Mutation
 - Random mutations to maintain diversity

 Step 6: Replacenent
 - Replace some or all of the old population with the new offspring

 Step 7: Repeat
 - Loop until the terminating criteria is reached