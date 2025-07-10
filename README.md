# Pricing_American_Options

---

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

- Computes American option prices using both:

   Polynomial regression (LSM_price)

   Laguerre polynomial regression (LSM_price_lg)

- Supports both American call and put options.

- Compares LSM prices with:

  Black-Scholes European option prices

  CRR Binomial and Trinomial American prices

- Analyzes convergence behavior with increasing number of Monte Carlo paths.

- Visualizes early exercise regions by tracking optimal stopping decisions.


