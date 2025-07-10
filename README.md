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

**Parameters Used:**
- $S_0 = 100$, $K = 100$, $T = 1.0$, $r = 5\%$, $\sigma = 20\%$

**Key Results:**
- American Put Price: \$6.7411
- European Put Price: \$6.4580 → Early Exercise Premium: **\$0.2831**
- American Call Price: \$9.4094
- European Call Price: \$9.4134 → Early Exercise Premium: **\$-0.0040**
- Estimated Convergence Rates:
  - Put: $O(1/n^{1.19})$
  - Call: $O(1/n^{1.24})$

