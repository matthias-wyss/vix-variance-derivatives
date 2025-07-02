# 🌪️ VIX and Variance Derivatives: Theory, Pricing, and Replication

This repository contains all the code, data, and derivations for the **Derivatives Project (FIN-404)** completed at EPFL in Spring 2025. The goal was to study and model volatility-related financial instruments, focusing on the **VIX index**, **variance swaps**, **futures**, and **replication techniques**.

## 📘 Project Summary

We develop a comprehensive understanding of volatility-linked derivatives through:

-  Derivation and interpretation of the **Carr-Madan replication formula**
-  Analytical and numerical treatment of the **VIX index** as a forward-looking measure of implied volatility
-  Pricing of **VIX and variance futures** using **affine models**
-  **Sensitivity analysis** of futures curves to model parameters (λ, θ, ξ)
-  **Calibration** of volatility dynamics to market prices
-  Replication of an SPX call using a portfolio of **variance and VIX futures**

The mathematical modeling follows a rigorous approach using **risk-neutral pricing**, stochastic calculus, and integral representations.

## 📂 Repository Structure

```
.
├── vix_and_var.ipynb                    # Main notebook with all derivations, formulas, and plots
├── derivatives-project-report.pdf       # Final report with full write-up and references
├── derivatives-project-guidelines.pdf   # Official project instructions and questions
├── Fin404-2025-VIXNCO-Data.xlsx         # Dataset used for calibration and pricing analysis
├── README.md                            # Project overview and instructions (this file)
└── requirements.txt (optional)          # Python dependencies if needed
```

## 🧠 Main Concepts Covered

- **Carr-Madan replication**
- **Log-payoff and power-payoff replication via vanilla options**
- **VIX derivation from OTM option prices**
- **Laplace transform and affine pricing of volatility futures**
- **Arbitrage between VIX and variance futures**
- **Static hedging of SPX options**

## 📈 Calibration Result (Example)

Volatility model parameters calibrated using market data:

```
λ = 1.30
θ = 0.0705
ξ = 0.260
Vₜ = 0.0498
```

These parameters allow accurate fitting of variance futures and partial replication of VIX futures.

## 🧪 Requirements

To run the notebook locally:

```bash
pip install numpy matplotlib scipy sympy pandas openpyxl
```

> Note: `openpyxl` is required to read `.xlsx` files.

## 📄 Documentation

- 📎 [`derivatives-project-report.pdf`](./derivatives-project-report.pdf): Full written report  
- 📎 [`derivatives-project-guidelines.pdf`](./derivatives-project-guidelines.pdf): Official assignment instructions  
- 📊 [`Fin404-2025-VIXNCO-Data.xlsx`](./Fin404-2025-VIXNCO-Data.xlsx): Dataset used for calibration and pricing

## 👥 Authors

- Matthias Wyss [@matthias-wyss](https://github.com/matthias-wyss)  
- William Jallot  
- Antoine Garin  
- Amine Bengelloun

**Course:** FIN-404 – Derivatives  
**Instructor:** Prof. Julien Hugonnier  
**Program:** EPFL – Master in Financial Engineering, Year 2