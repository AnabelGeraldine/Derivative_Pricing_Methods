# Derivative_Pricing_Methods

## Objective
The goal of this project is to analyze and implement pricing models for financial derivatives, focusing on Monte Carlo simulations and Finite Difference Methods (FDM). These numerical techniques are crucial in valuing complex derivatives, particularly in cases where analytical solutions like the Black-Scholes model are not feasible. The study aims to compare the accuracy, efficiency, and computational performance of these two methods in pricing options under different market conditions.

## Methods and Tools Used
The project was implemented using Python, utilizing libraries such as NumPy, SciPy, and Matplotlib for numerical computations and visualization. The methods used include:

### Monte Carlo Simulations (MC):

- Simulated multiple price paths for an underlying asset using Geometric Brownian Motion (GBM).
- Generated thousands of random price trajectories to estimate the expected option payoff.
- Applied risk-neutral valuation by discounting the average payoff back to the present.

### Finite Difference Methods (FDM):

- Used explicit, implicit, and Crank-Nicholson schemes to numerically solve partial differential equations (PDEs) governing option pricing.
- Discretized the option pricing equation on a grid to approximate the derivative price evolution over time.
### Model Evaluation:

- Compared accuracy, convergence speed, and computational cost of both methods.
- Assessed performance across European and American options to determine practical applicability.
## Findings and Conclusion
The analysis found that Monte Carlo methods are more flexible and suitable for pricing derivatives with complex payoffs and multiple sources of uncertainty, such as exotic options. However, MC simulations are computationally expensive and slow to converge, requiring variance reduction techniques for improved efficiency. On the other hand, Finite Difference Methods provided more precise and stable results for simpler derivative structures like European options, particularly with the Crank-Nicholson method balancing stability and accuracy. The study concludes that Monte Carlo methods are preferable for high-dimensional problems, while FDM is well-suited for simpler derivatives with fewer state variables. Future work could explore optimization techniques for both methods, such as parallelization in Monte Carlo and adaptive meshing in Finite Difference Methods, to enhance computational efficiency.
