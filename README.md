# KF-Beta-Momentum 📈

A dynamic equity allocation strategy combining **Kalman Filter-based time-varying beta estimation** with **momentum-driven alpha signals** under explicit risk constraints.

---

## 📌 Project Overview

This project implements a rigorous quantitative backtesting framework with the following core components:

- **Dynamic Beta Estimation**
  - Uses a Kalman Filter to estimate time-varying betas for 300 CSI 300 constituent stocks relative to the benchmark index.

- **Momentum-Based Alpha Signal**
  - Constructs alpha signals using a 20-day rolling cumulative return (short-term momentum).

- **Risk-Constrained Portfolio Optimization**
  - Solves a constrained optimization problem under:
    - Fully invested constraint
    - Long-only position limits
    - Target portfolio beta band: **[0.95, 1.05]**

- **Realistic Return Modeling**
  - Incorporates time-varying risk-free rates (Shibor-based) to compute excess and total returns consistently.

---

## 📊 Strategy Performance (2021–2026)

| Metric | Value |
|:------|------:|
| Annualized Return | **41.32%** |
| Information Ratio | **1.31** |
| Sharpe Ratio | **1.03** |
| Maximum Drawdown | **-54.26%** |

---

## 🧪 Tech Stack

- Python 3.11
- NumPy / Pandas
- SciPy (optimization)
- Matplotlib
---
