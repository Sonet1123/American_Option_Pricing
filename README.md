# American Option Pricing

This project implements and compares multiple numerical methods for pricing American-style options, focusing on early exercise features and convergence behavior. The methods include tree-based models (CRR Binomial, Trinomial Tree), simulation-based Least Squares Monte Carlo (LSM), and Finite Difference Methods (Explicit, Implicit, Crank-Nicolson). For each approach, both American call and put options are examined and benchmarked against the European Black-Scholes price.

### Module 1: American Option Pricing Using CRR Binomial Tree
This module implements the Cox-Ross-Rubinstein (CRR) binomial tree method to price American call and put options.

**Highlights:**
- Early exercise handled via backward induction
- Both American and European prices computed
- Early exercise premium quantified
- Convergence analysis performed and visualized
- Early exercise regions plotted

### Module 2: American Option Pricing – Trinomial Tree Method
This module implements American option pricing using a recombining Trinomial Tree. Both call and put options are evaluated.

Key components include:
- Accurate pricing with early exercise handling
- Comparison with Black-Scholes European prices
- Convergence analysis with plots
- Estimation of convergence rate
- Visualization of early exercise region

### Module 3: Least-Squares Monte Carlo (LSM)
This module implements American option pricing using the Least-Squares Monte Carlo (LSM) method introduced by Longstaff and Schwartz (2001). The continuation value is estimated via regression on simulated paths using two types of basis functions: standard polynomials and Laguerre polynomials.

#### Features
- Simulates multiple price paths using geometric Brownian motion.
- Computes American option prices using both: Polynomial regression (LSM_price), Laguerre polynomial regression (LSM_price_lg)
- Supports both American call and put options.
- Compares LSM prices with: Black-Scholes European option prices, CRR Binomial and Trinomial American prices
- Analyzes convergence behavior with increasing number of Monte Carlo paths.
- Visualizes early exercise regions by tracking optimal stopping decisions.


## Module 4: Finite Difference Methods for American Put Options

This module implements and compares three numerical PDE-based methods to price American put options:

###  Methods Implemented
- **Explicit Finite Difference Method** (backward-Time Centered-Space)
- **Implicit Finite Difference Method** (Forward-Time Centered-Space with PSOR)
- **Crank-Nicolson Method** (Averaged scheme with PSOR)

###  Features
- Accurate pricing of American-style options under early exercise constraints
- Comparison of option prices with CRR Binomial and Black-Scholes European values
- Convergence analysis for each method
- Visualization of the early exercise region


### Notes
- PSOR (Projected Successive Over-Relaxation) is used in Implicit and CN schemes to handle the free boundary.
- Crank-Nicolson shows good accuracy but convergence may degrade due to the early exercise constraint.

## Files
- `main.ipynb` — Jupyter notebook to implement
- `pricing_american_options.pdf` — Project report 


