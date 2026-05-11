# GoF-Framework-Symmetry
### A Goodness-of-Fit Framework for Assessing Distributional Symmetry and Tail Asymmetry in Financial Equity Markets

This repository contains the official Python implementation of the multi-stage econometric framework proposed in the study: **"A Goodness-of-Fit Framework for Assessing Distributional Symmetry and Tail Asymmetry in Financial Equity Markets"**.

The project moves beyond linear correlation by utilizing non-parametric Goodness-of-Fit (GoF) tests, Energy Distance metrics, and Extreme Value Theory (EVT) to diagnose structural risk and tail asymmetries in financial assets.

## 🚀 Key Features

- **ARMA-GARCH Filtering:** Automated extraction of standardized IID innovations to ensure statistical validity of GoF tests.
- **GoF Testing Suite:** Implementation of Kolmogorov-Smirnov (KS), permutation-based Anderson-Darling (AD), and Epps-Singleton (ES) tests.
- **Energy Distance Decomposition:** Separation of structural divergence ($ED_{Shape}$) from scale-driven volatility ($ED_{Scale}$).
- **Extreme Risk Profiling:** Tail index estimation (1% and 5% thresholds) using Extreme Value Theory and robust L-Moments.
- **Risk-Based Clustering:** Hierarchical Agglomerative Clustering to categorize assets into Safe Haven, Gray Zone, and Toxic risk profiles.
- **Economic Validation:** A 1,000-iteration bootstrapped portfolio backtesting engine to compare GoF-based strategies against random allocations.

## 🛠 Tech Stack

- **Language:** Python 3.10+
- **Key Libraries:**
  - `arch`: For ARMA-GARCH modeling and maximum likelihood estimation.
  - `scipy`: For statistical distributions and classical GoF tests.
  - `numpy` & `pandas`: For vectorized data manipulation and numerical stability.
  - `scikit-learn`: For hierarchical clustering and manifold learning.
  - `matplotlib` & `seaborn`: For high-quality KDE overlaps and clustering visualizations.

## 📋 Methodology Overview

The framework operates in five distinct stages:
1. **Stage 1 (Benchmark Symmetry):** Analyzing individual stocks against market proxies (e.g., S&P 500).
2. **Stage 2 (Sectoral Alignment):** Comparing assets against their respective sectoral ETFs (XLK, XLE, XLP, etc.).
3. **Stage 3 (Tail Dynamics):** EVT-based tail indices and L-moment decomposition.
4. **Stage 4 (Hierarchical Clustering):** Mapping risk taxonomies based on $ED_{Shape}$ and $L_{Kurtosis}$.
5. **Stage 5 (Economic Proof-of-Concept):** Validating risk-adjusted returns via bootstrapped backtesting.

## 💻 Installation

```bash
# Clone the repository
git clone [https://github.com/asevin85/GoF-Framework-Symmetry.git](https://github.com/asevin85/GoF-Framework-Symmetry.git)

# Install required packages
pip install numpy pandas scipy arch scikit-learn matplotlib seaborn

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

✉️ Contact
Abdullah Sevin - asevin@sakarya.edu.tr
Project Link: https://github.com/asevin85/GoF-Framework-Symmetry
