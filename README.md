# Solving NxNxN Rubik Cube in Optimal Way 🧩

This project aims to explore various approaches to solving an NxNxN Rubik Cube, focusing on both brute force and optimal algorithms. The project is divided into three main parts:

## Part 1: Prove the NP-Completeness of NxNxN Rubik Cube 🧠
https://drops.dagstuhl.de/storage/00lipics/lipics-vol096-stacs2018/LIPIcs.STACS.2018.24/LIPIcs.STACS.2018.24.pdf

In this section, we demonstrate that solving an NxNxN Rubik Cube is an NP-complete problem. This involves proving that the problem is both in NP (i.e., a solution can be verified quickly) and that it is at least as hard as other known NP-complete problems, such as the 3-SAT problem. We explore the complexity of different cube sizes and show that the difficulty of solving the puzzle grows exponentially as the number of cube dimensions increases.

Key points covered:
- Explanation of NP-completeness 💡
- Mapping the Rubik Cube problem to an NP-complete problem 🔍
- Proof that solving the NxNxN Rubik Cube requires significant computational effort as the size of the cube increases ⚙️

## Part 2: Algorithms to Solve NxNxN Rubik Cube 💻

In this section, we explore multiple algorithms to solve the NxNxN Rubik Cube, including both brute-force and optimal solutions.

### Brute Force Algorithm 🛠️

A brute force algorithm tries every possible configuration of the cube until it finds the correct one. This approach is highly inefficient, but it serves as a baseline comparison for optimal methods. The brute force approach demonstrates the impracticality of solving large Rubik cubes due to the astronomical number of possible states.

- **Time complexity**: Exponential, dependent on the size of the cube ⏳
- **Memory complexity**: High, since it needs to store multiple configurations at once 💾

### Optimal Algorithms 🎯

#### 1. **Korf's (IDA*) 🚀**
Finding optimal solutions to Rubik's cube using pattern databases


#### 2. **DeepCubeA 🚀**
https://www.nature.com/articles/s42256-019-0070-z#citeas

#### 3. **Kociemba's Algorithm (Two-Phase Algorithm) 🚀**
https://github.com/hkociemba/RubiksCube-OptimalSolver/tree/master
The first optimal algorithm is Kociemba's two-phase algorithm. This method splits the problem into two phases:
- **Phase 1**: Solve a simplified version of the cube (reduced group of moves).
- **Phase 2**: Complete the solution using a smaller set of moves to solve the cube optimally.

Kociemba's algorithm is widely regarded as one of the most efficient methods for solving the Rubik Cube in terms of the number of moves required.

- **Time complexity**: Polynomial ⏱️
- **Space complexity**: Polynomial 🧮

#### 4. **Thistlethwaite's Algorithm 🧩**

Thistlethwaite's algorithm reduces the cube’s complexity by breaking it down into groups, solving each one in stages:
- **Stage 1**: Simplify the cube using group theory 🧠
- **Stage 2**: Solve the cube using minimal moves for each group 🏁

Thistlethwaite’s method guarantees an optimal solution and involves fewer moves compared to the brute-force approach, but can be more computationally intensive than Kociemba’s.

- **Time complexity**: Polynomial ⏱️
- **Space complexity**: Polynomial 🧮

## Part 3: Custom Algorithm for Solving NxNxN Rubik Cube 🔧

In this section, we introduce a custom algorithm designed to solve the NxNxN Rubik Cube more efficiently than the brute-force approach while still achieving an optimal solution. Our custom algorithm combines elements of group theory with heuristic optimizations, reducing the search space for possible solutions.

Key improvements:
- **Heuristics**: Uses domain-specific heuristics to prioritize promising configurations and reduce the number of states explored 🔍
- **Parallelization**: Implements parallel processing to solve the cube faster by exploring multiple branches of the solution space simultaneously ⚡
- **Optimized Move Strategy**: Implements advanced move strategies to minimize the number of steps required to reach the solved state 🔄

### Time and Space Complexity ⏳💡

- **Time complexity**: Reduced compared to brute force, closer to polynomial time ⏱️
- **Space complexity**: Efficient use of memory due to optimized data structures 💾

## Conclusion 🏁

This project demonstrates the complexity of solving the NxNxN Rubik Cube and explores different algorithmic approaches, from brute force to highly optimized methods. By developing both a theoretical and practical understanding of solving Rubik’s Cubes, we can apply these techniques to other problems in computational complexity and optimization.

## Acknowledgements 🙏

- The algorithms referenced in this project are based on the works of [Herbert Kociemba](https://kociemba.org/) and [Michael Thistlethwaite](http://www.math.utk.edu/~thistle/).
- Thanks to open-source Rubik's Cube solver libraries and contributors for providing a foundation to build on. 
