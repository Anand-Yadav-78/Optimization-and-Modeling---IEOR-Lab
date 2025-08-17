# **Optimization-and-Modeling---IEOR-Lab**

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

# **Applied-Optimization-and-Modeling-Labs**

This repository serves as a portfolio of various computational optimization projects, demonstrating the application of a wide range of techniques. The project consolidates several lab exercises into a unified showcase, covering gradient-based methods for high-dimensional problems, financial portfolio optimization, and solving the combinatorial Vehicle Routing Problem (VRP).

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

# **📋 Problem Statement**
This repository addresses a series of distinct optimization challenges to demonstrate the practical application and comparative performance of various algorithms. The core objective is to select the appropriate modeling technique for each problem class, implement a robust solution, and analyze the results in terms of efficiency, scalability, and solution quality. The problems tackled include:

Unconstrained Non-Linear Optimization: Minimizing a high-dimensional objective function and comparing the performance of different gradient-based methods.

Portfolio Optimization: Constructing an optimal stock portfolio to balance risk and return under a fixed budget.

Vehicle Routing Problem (VRP): Finding the shortest possible routes for a fleet of vehicles to serve a set of customers, comparing exact and heuristic methods.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

# **📊 Data Summary**
The analysis utilizes several distinct datasets and functions tailored to each optimization problem:

High-Dimensional Objective Function: A complex, non-linear function f(x) = Σ[4(xᵢ₊₁ - xᵢ²)² + (xᵢ - 1)²] is used to test the scalability of unconstrained optimization algorithms on dimensions (n) up to 10,000.

Portfolio Optimization Data: Historical stock data is used to compute the mean return vector (μ) and the covariance matrix (Σ) for a selection of stocks, forming the basis for mean-variance optimization.

Vehicle Routing Problem Data: A classic VRP instance with a central depot, 11 demand points, and a vehicle capacity of 100 units.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

# **🛠️ Methodology & Techniques**
A diverse set of optimization techniques was implemented and compared across the different exercises, showcasing a versatile problem-solving toolkit.

Gradient-Based Unconstrained Optimization:

Steepest Descent with a backtracking line search to investigate the impact of initial step sizes.

BFGS (Quasi-Newton Method) to demonstrate efficient convergence for high-dimensional problems without requiring explicit Hessian calculations.

Newton's Method with an exact Hessian (and pseudoinverse for stability) to achieve quadratic convergence.

Comparative Analysis: A direct comparison of the computational time and scaling properties (linear vs. quadratic vs. cubic) of these methods.

Financial Portfolio Optimization:

Mean-Variance Optimization: Formulated as a Quadratic Program (QP) to find the portfolio with the minimum risk for a given level of expected return.

Baseline Comparison: The performance of the optimized portfolio is benchmarked against a naive equal-allocation strategy.

Combinatorial Optimization (VRP):

Exact Method: Solved using Google OR-Tools, a powerful library with specialized algorithms like guided local search.

Heuristic Methods: Implemented and compared Simulated Annealing (SA) and a Genetic Algorithm (GA) as alternative, approximate solution methods.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

# **🚀 Tools and Libraries**
This project was built using Python and the following core scientific computing and optimization libraries:

NumPy & SciPy: For numerical operations, vector/matrix algebra, and scientific computations.

Pandas: For data manipulation in the portfolio optimization task.

Google OR-Tools: A specialized, high-performance library for solving combinatorial optimization problems like the VRP.

Matplotlib: For data visualization and plotting performance comparisons.

PuLP / CVXPY (Inferred): Standard Python libraries for formulating and solving the quadratic program in the portfolio optimization exercise.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

# **💡 Inference and Conclusion**
The consolidated analysis across these exercises yielded several key insights into the practical application of optimization algorithms.

Scalability Trade-Offs: The comparison of gradient-based methods clearly demonstrated the trade-off between per-iteration cost and convergence rate. While Newton's method converges in fewer steps, its cubic (O(n³) ) complexity makes it less practical for very large dimensions compared to the quadratic (O(n²)) scaling of BFGS.

Superiority of Specialized Solvers: For the Vehicle Routing Problem, the specialized algorithms within Google OR-Tools consistently provided higher-quality solutions in less time than the general-purpose heuristics (Simulated Annealing and Genetic Algorithms).

Value of Quantitative Finance: The portfolio optimization exercise proved that a quantitative, mean-variance approach produces a portfolio with a significantly better risk-return profile than a naive equal-allocation strategy, highlighting the value of optimization in financial decision-making.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

# **Final Conclusion:**
This project serves as a practical demonstration of a versatile optimization toolkit, showcasing the ability to formulate, implement, and analyze algorithms for a wide range of problem classes. It highlights the importance of selecting the right tool for the task—from choosing an appropriate gradient method based on problem dimensionality to leveraging specialized solvers for complex combinatorial problems. The findings underscore the critical role of computational optimization in solving real-world challenges in engineering, finance, and logistics.
