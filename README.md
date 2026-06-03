#  Optimal Power Flow (OPF) Optimization
OPF implementation for economic load dispatch and power system optimization.


This project focuses on solving the **Optimal Power Flow (OPF)** problem in smart power grids to minimize generation cost while maintaining system stability, voltage limits, and transmission constraints.

The project is implemented using metaheuristic optimization techniques such as:
- Genetic Algorithm (GA)
- Tabu Search (TS)
- Simulated Annealing (SA)

The performance of these algorithms is evaluated on the IEEE 14-bus test system.

---


## Project Objective

The goal of this project is to optimize power system operation by:
- Minimizing total generation cost and transmission losses  
- Maintaining voltage stability across all buses  
- Ensuring system constraints satisfaction  
- Improving integration of renewable energy sources  
- Enhancing grid reliability and efficiency  

---

## Test System

- IEEE 14-Bus Power System  
- 14 Buses, 5 Generators, 11 Loads, 20 Transmission Lines  
- Standard benchmark system for OPF studies  
- Used for comparison of optimization algorithms  

---

## Optimization Techniques Used

###  Genetic Algorithm (GA)
A population-based evolutionary algorithm inspired by natural selection used to find near-optimal OPF solutions.

**Key Steps:**
- Initialization of population
- Fitness evaluation (cost minimization + constraints)
- Selection of best solutions
- Crossover and mutation
- Iterative improvement until convergence

---

###  Tabu Search (TS)
An iterative local search algorithm that avoids revisiting recent solutions using memory (tabu list).

**Key Steps:**
- Initial feasible solution
- Neighborhood generation
- Evaluation of candidate solutions
- Tabu list update
- Aspiration criteria for better solutions
- Iterative improvement

---

###  Simulated Annealing (SA)
A probabilistic optimization technique that allows exploration of worse solutions early to avoid local minima.

**Key Steps:**
- Initial solution & temperature setup
- Neighbor generation
- Probabilistic acceptance function
- Cooling schedule
- Iterative optimization until convergence

Acceptance Probability:
\[
P = e^{-\Delta / T}
\]

---

## 📐 Mathematical Formulation

### Objective Function
Minimize total generation cost:
\[
\min \sum C_i(P_i)
\]

---

### Constraints

**Power Balance Constraints:**
- Active power balance
- Reactive power balance

**Voltage Constraints:**
\[
V_{min} \leq V_i \leq V_{max}
\]

**Transmission Line Limits:**
- Power flow must not exceed thermal limits

---

## Implementation Details

- Programming Language: Python  
- Simulation System: IEEE 14-bus system  
- Optimization Methods: GA, TS, SA  
- Tools: NumPy, Matplotlib, optimization libraries  

---

##  Results & Observations

- Optimal generation dispatch achieved  
- Reduction in total generation cost  
- Voltage profile maintained within limits  
- Comparison of GA, TS, and SA performance  
- Effective constraint handling observed  

---
 

## Repository Contents

- OPF_Optimization_IEEE14.ipynb  
- Simulation results  
- Graphs and plots  
- Project report PDF  
- README documentation  

---

## References

- IEEE 14-Bus Test System (PSTCA / ICSEG)  
- GeeksforGeeks – Simulated Annealing  
- Cornell Optimization Notes  
- Lecture Notes on Tabu Search  
- Metaheuristic Optimization Methods in Power Systems  

---
