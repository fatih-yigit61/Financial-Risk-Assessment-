# Financial Risk Analysis with Fixed-Point Iteration

This project presents a financial risk analysis tool that uses **fixed-point iteration** to compute **equilibrium interest rates** based on key economic indicators. It focuses on the **United States economy between 1992 and 2008** and evaluates financial stability by classifying interest rates into risk categories.

## Project Objective

To assess financial risk levels in a systematic and dynamic way by:
- Computing equilibrium interest rates using fixed-point iteration.
- Integrating economic indicators such as GDP growth, inflation, government expenditure, and public bonds.
- Visualizing trends and risk levels over time.

## Methodology

1. **Data Collection**
   - Economic datasets from the World Bank (1992–2008).
   - Indicators used:
     - Public Bonds
     - Inflation
     - Government Expenditure
     - GDP Growth

2. **Fixed-Point Iteration**
   - Iteration Formula: `g(x) = 0.85x + 0.15 * economic_indicator`
   - Starts from `x₀ = 5` and continues until:
     - Convergence threshold: `|x(n+1) - x(n)| < 1e-6`
     - Or maximum iterations (100)

3. **Risk Classification**
   - Equilibrium interest rates are mapped to risk levels:
     - `> 30`: Critical Risk
     - `20–30`: High Risk
     - `12–20`: Medium Risk
     - `5–12`: Low Risk
     - `≤ 5`: Very Low Risk

4. **Visualization**
   - Line plots of stable interest rates by dataset
   - Bar charts showing risk level trends
   - Convergence plots showing number of iterations

## Outputs

- **Equilibrium Interest Rate Trends** for each dataset.
- **Risk Level Annotations** directly on the plots.
- **Iterations-to-Convergence** visual analysis.
- **Combined and comparative graphs** across economic indicators.
