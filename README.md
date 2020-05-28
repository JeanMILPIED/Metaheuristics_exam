# Metaheuristics_exam
my work for DSTI A19 metaheuristics exam

## 1. structure of the reports
In each folder, one can find the python Jupyter notebook to run the optimisation of the problem, and the image of the solutions.   
The solutions to the problems are shared in this readme.  
the python packages used are numpy, pandas, scipy.optimize

## 2. Problem solutions
### 2.1 TSP - Djibouti
The thinking process is highly described in the Jupyter notebook.  
For this discrete optimisation problem, we used a a random 2 by 2 swap home coded algorithm encapsulated in a simulated annealing shell to overcome local minima. Everything was coded in numpy array to optimize compute cost.  
The best solution found is:  
- cost: 6659
- time computing: <1min
![TSP-Djibouti solution](/1.%20TSP%20djibouti/TSP%5E_djibouti.PNG)

### 2.2 TSP - Qatar
The same algorithm as for Djibouti is used.  
The performance achieved is correct with smart initialisation + generation of random solutions + SImulated annealing to overcome local mimimums.  
The best solution found is:  
- cost: 10582
- time computing: 14min
![TSP-Qatar solution](/2.%20TSP%20Qatar/TSP_qatar.PNG)

### 2.3 F1 - Shifted Sphere Function
This is a linear and derivable function. We use a simple minimize function with gradient algo.
Results are given hereunder:  
- for D=50:


- for D= 500:




### 2.4 F2 - Shifted Schwefel’s Problem 2.21
This is a continuous function with a global minimum, but not derivable at this optimum. Nevertheless, we use a minimize function with gradient descent algorithm.  
Results are given hereunder: 
- for D=50:


- for D= 500:


### 2.5 F3 - Shifted Rosenbrock’s Function
This is a continuous function with a global minimum but also having a very narrow valley from local optimum to global optimum. This may affect the performance of the gradient descent optimization algorithm. Nevertheless we keep using a minimize function here.  
Results are given hereunder: 
- for D=50:


- for D= 500: we don't achieve to get to the global optimum.

### 2.6 F4 - Shifted Rastrigin’s Function
This is a continuous function with a global optimum but Local optima’s number is huge. We prefer here to use a genetic algorithm to more quickly converge towards the optimum solution.
Results are given hereunder: 
- for D=50:


- for D= 500:

### 2.7 F5 - Shifted Griewank’s Function


### 2.8 F6 - Shifted Ackley’s Function


