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

### Continuous optimization synthesis table

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
![F1 dim 50](/3.%20F1%20Sphere/F1_50.PNG)  
  
- for D= 500:  
![F1 dim 500](/3.%20F1%20Sphere/F1_500_1.PNG)  
![F1 dim 500_2](/3.%20F1%20Sphere/F1_500_2.PNG)  
  
### 2.4 F2 - Shifted Schwefel’s Problem 2.21
This is a continuous function with a global minimum, but not derivable at this optimum. Nevertheless, we use a minimize function with gradient descent algorithm.  
Results are given hereunder: 
- for D=50:  
![F2 dim 50](/4.%20F2/F2_50.PNG)  

- for D= 500:  
![F2 dim 500](/4.%20F2/F2_500_1.PNG)  
![F2 dim 500_2](/4.%20F2/F2_500_2.PNG)  
  
### 2.5 F3 - Shifted Rosenbrock’s Function
This is a continuous function with a global minimum but also having a very narrow valley from local optimum to global optimum. This may affect the performance of the gradient descent optimization algorithm. Nevertheless we keep using a minimize function here.  
Results are given hereunder: 
- for D=50:  
![F3 dim 50](/5.%20F3/F3_50_1.PNG)  
![F3 dim 50_2](/5.%20F3/F3_50_2.PNG)   

- for D= 500: we don't achieve to get to the global optimum.  
![F3 dim 500](/5.%20F3/F3_500_1.PNG)  
![F3 dim 500_2](/5.%20F3/F3_500_2.PNG) 

### 2.6 F4 - Shifted Rastrigin’s Function
This is a continuous function with a global optimum but Local optima’s number is huge. We prefer here to use a genetic algorithm to more quickly converge towards the optimum solution.
Results are given hereunder: 
- for D=50:  
![F4 dim 50](/6.%20F4/F4_50_1.PNG)  
![F4 dim 50_2](/6.%20F4/F4_50_2.PNG)

- for D= 500: we don't achieve to run this in apporopriate time...


### 2.7 F5 - Shifted Griewank’s Function
This is a continuous function and the challenge is here in the very broad range of values.  
We prefer continuing with a GA optimization algorithm.
Results are given hereunder: 
- for D=50:  
![F5 dim 50](/7.%20F5/F5_50_1.PNG)
![F5 dim 50_2](/7.%20F5/F5_50_2.PNG)  

- for D= 500:  



### 2.8 F6 - Shifted Ackley’s Function
This is a continuous function with a sharp optimum where gradients are very high and not differentiable at the global optimum.  
We apply GA for this optimiation problem too.
Results are given hereunder: 
- for D=50:  
![F6 dim 50](/8.%20F6/F6_50_1.PNG)  
![F6 dim 50_2](/8.%20F6/F6_50_2.PNG)


- for D= 500:


