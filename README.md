

# Rubik's Cube Solver Using Korf's IDA Algorithm  

This project implements a Rubik's Cube solver using Korf's Iterative Deepening (IDA) algorithm. The goal of the solver is to efficiently find the optimal solution to a scrambled Rubik's Cube, minimizing the number of moves required. This approach is based on the heuristic search techniques described by Richard Korf, specifically tailored for solving combinatorial puzzles like the Rubik's Cube.  

## Project Overview  

The Rubik's Cube is a complex puzzle with over 43 quintillion possible states. Finding the optimal solution requires sophisticated algorithms that can navigate this immense search space. Korf's IDA algorithm combines the benefits of depth-first search and heuristic estimates to iteratively explore possible moves. The algorithm terminates once the shortest solution is identified.  

This project includes both the implementation of the algorithm and a framework to simulate the Rubik's Cube. The code is designed to take a scrambled cube state as input and return the sequence of moves required to solve it.  

## Features  

- Implementation of the IDA algorithm with heuristic-based pruning.  
- Simulation of the Rubik's Cube, including basic rotations and state validation.  
- Optimized data structures for efficient state representation and manipulation.  
- Clear modular design to extend or adapt the solver for future improvements.  

## How It Works  

1. **Cube Representation**: The cube is represented in a way that allows efficient manipulation of its state. Each face of the cube is assigned unique identifiers for easy tracking.  
2. **Heuristic Function**: A heuristic is used to estimate the minimum number of moves required to solve the cube from any given state.  
3. **Iterative Deepening**: The algorithm starts with a move limit and increases it incrementally. Within each iteration, it explores all possible moves up to the current limit using depth-first search.  
4. **Optimal Solution**: Once the algorithm finds a solution within the current move limit, it halts and outputs the sequence of moves.  

## How to Use  

1. Clone the repository to your local machine:  
   ```bash  
   git clone https://github.com/your-username/Rubik-Cube-Solver.git  
   ```  
2. Install the necessary dependencies, if any (refer to the requirements file or project setup instructions).  
3. Run the main script and provide the scrambled cube state as input. The program will output the solution sequence.  

## Applications  

This solver can be used for research purposes, as a learning tool for understanding heuristic algorithms, or as a component in robotics projects where solving a Rubik's Cube is required.  

## Future Enhancements  

- Implement graphical visualization of the cube and its solution process.  
- Explore alternative heuristics to improve computational efficiency.  
- Extend the solver to handle larger puzzles, such as 4x4 or 5x5 cubes.  

## Conclusion  

This project demonstrates the power of heuristic search algorithms in solving complex combinatorial problems. By using Korf's IDA* algorithm, the solver achieves an optimal solution in a reasonable time frame, showcasing the elegance and efficiency of this approach.  

