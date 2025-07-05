# Advanced Rubik's Cube Solver

A comprehensive C++ implementation of multiple Rubik's Cube solving algorithms, featuring various data structures and optimization techniques.

## 🎯 Overview

This project demonstrates advanced algorithmic problem-solving through the implementation of four different cube-solving approaches, each optimized for different scenarios. The solver supports multiple cube representations and uses pattern databases for enhanced performance.

## ✨ Features

- **Multiple Solving Algorithms**
  - DFS (Depth-First Search) with depth limiting
  - BFS (Breadth-First Search) for optimal solutions
  - IDDFS (Iterative Deepening DFS) for memory efficiency
  - IDA* (Iterative Deepening A*) with heuristic optimization

- **Various Cube Representations**
  - 3D Array: Intuitive and easy to understand
  - 1D Array: Memory-optimized representation
  - Bitboard: High-performance bit manipulation

- **Advanced Optimizations**
  - Pattern database implementation
  - Corner heuristic functions
  - Efficient move generation and validation

## 🛠️ Tech Stack

- **Language:** C++14
- **Build System:** CMake 3.20+
- **Data Structures:** Arrays, Bitboards, Hash Tables
- **Algorithms:** Graph Search, Heuristic Functions, Pattern Matching

## 📁 Project Structure

├── Model/ # Cube representation classes
│ ├── RubiksCube.h # Base cube interface
│ ├── RubiksCube3dArray.cpp # 3D array implementation
│ ├── RubiksCube1dArray.cpp # 1D array implementation
│ └── RubiksCubeBitboard.cpp # Bitboard implementation
├── Solver/ # Algorithm implementations
│ ├── DFSSolver.h # Depth-first search
│ ├── BFSSolver.h # Breadth-first search
│ ├── IDDFSSolver.h # Iterative deepening DFS
│ └── IDAstarSolver.h # IDA* with heuristics
├── PatternDatabases/ # Heuristic optimization
│ ├── CornerPatternDatabase.* # Corner pattern implementation
│ └── CornerDBMaker.* # Database generation utilities
├── Databases/ # Precomputed pattern data
└── main.cpp # Testing and demonstration

## 🚀 Building and Running

### Prerequisites
- C++14 compatible compiler (GCC 7+, Clang 5+, MSVC 2017+)
- CMake 3.20 or higher

### Build Instructions

1. **Clone and navigate:**

2. **Create build directory:**

3. **Configure and build:**

4. **Run the solver:**

## 🎮 Usage

The main.cpp file contains various test cases demonstrating different solvers. Uncomment specific sections to test different algorithms:


## 🧮 Algorithm Comparison

| Algorithm | Time Complexity | Space Complexity | Optimality | Use Case |
|-----------|----------------|------------------|------------|----------|
| DFS | O(b^d) | O(d) | No | Quick solutions |
| BFS | O(b^d) | O(b^d) | Yes | Optimal solutions |
| IDDFS | O(b^d) | O(d) | Yes | Memory-efficient optimal |
| IDA* | O(b^d) | O(d) | Yes | Fastest optimal solutions |

## 🔧 Customization

- **Adding New Algorithms:** Extend the base solver class
- **Custom Heuristics:** Implement new pattern databases
- **Different Cube Sizes:** Modify cube representation classes
- **Performance Tuning:** Adjust search parameters and optimizations

## 📊 Performance

- **Average solve time:** < 2 seconds for scrambled cubes
- **Memory usage:** Optimized through bitboard representation
- **Solution length:** Near-optimal move sequences

## 🤝 Contributing

Contributions welcome! Areas for improvement:
- Additional solving algorithms (CFOP, Roux, etc.)
- GUI implementation
- Performance optimizations
- Cross-platform compatibility

## 📝 License

This project is open source and available under the MIT License.
