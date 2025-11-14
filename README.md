# [**Applied Statistics**](https://en.wikipedia.org/wiki/Statistics#Applied_statistics,_theoretical_statistics_and_mathematical_statistics)

<!--Study of the practical use of statistical methods to collect, analyse, interpret, and present data in real-world contexts.-->

This repository contains my official submission for the **Applied Statistics** assessment.  
It is structured, documented, and reproducible — providing a clear demonstration of statistical understanding and computational implementation.

All finalised solutions and explanations are contained within the main notebook:  
**[`problems.ipynb`](./problems.ipynb)**  

No rough work or exploratory notebooks are included here; all drafts are kept locally.

---

## Overview & Purpose

The [**Applied Statistics**](https://atu.ie) module enables students to demonstrate their ability to:

1. **Describe** the stochastic nature of real-world measurements.  
2. **Source documentation** to programmatically perform a statistical test.  
3. **Select** the appropriate statistical test to investigate a claim.  
4. **Perform** a statistical test on a dataset and interpret the results.

This repository serves as a single, self-contained record of work aligned with these learning outcomes.

---

## Codespaces Environment — *Improved Telegram*

This repository is hosted and developed in [**GitHub Codespaces**](https://docs.github.com/en/codespaces/quickstart), under the workspace named **“improved telegram”**.

By default, a Codespace development environment runs on a **virtual machine (VM)** based on [**Ubuntu Linux**](https://en.wikipedia.org/wiki/Ubuntu#:~:text=Ubuntu%20can%20be%20installed%20directly,for%20platforms%20such%20as%20OpenStack.) and includes many popular tools and languages.  
This setup ensures a consistent, cloud-based environment regardless of your local operating system.

**Key features:**

- Runs entirely in a **Linux (Ubuntu)** environment.  
- Compatible with **Python, Jupyter, [Git](https://git-scm.com/), and command-line utilities** preinstalled.  
- You can extend or customise the base image with additional libraries or tools.  
- Windows and macOS are *not* supported as remote container OS options — all Codespaces execute within Linux.  
- Ideal for running notebooks, simulations, and data visualisations directly in the browser.

This approach ensures maximum reproducibility, consistency, and ease of collaboration.

---

## Guidance & Structure

All work is presented in a single Jupyter Notebook: problems.ipynb.
Each problem section includes:

A short plan/approach (Markdown).

Code cells with clear structure and comments.

Outputs and plots with readable labels.

A brief interpretation and discussion of results.

Headings are consistent and sequential:

**# Applied Statistics** (title) → **## Problem 1**, **## Problem 2**, etc.

---

## Repository Structure

```bash
├── README.md             # This file — overview, purpose, and guidance
├── problems.ipynb        # Main notebook with all solutions (assessment focus)
├── requirements.txt      # Minimal reproducible environment
├── .gitignore            # Python + Jupyter configuration
├── data/                 # (Optional) small datasets if required
├── images/               # Exported plots or figures
└── roughwork/            # Not included here (kept locally only)


```

---
## Requirements

- [ipython](https://pypi.org/project/ipython/)
- [numpy](https://pypi.org/project/numpy/)
- [scipy](https://pypi.org/project/scipy/)
- [statsmodels](https://pypi.org/project/statsmodels/)
- [matplotlib](https://pypi.org/project/matplotlib/)
- [pandas](https://pypi.org/project/pandas/)
- [seaborn](https://pypi.org/project/seaborn/)
- [sympy](https://pypi.org/project/sympy/)
- [nose](https://pypi.org/project/nose/)
- [scikit-learn](https://pypi.org/project/scikit-learn/)
- [qiskit[visualization]](https://pypi.org/project/qiskit/)
- [yfinance](https://pypi.org/project/yfinance/)

---

## Problems Overview

Problem 1 — Extending the Lady Tasting Tea

Estimate the probability of correctly identifying all cups under random guessing for 12 cups (8 tea-first, 4 milk-first).
Compare with the classic 8-cup (4 vs 4) case and discuss implications for p-value thresholds.

Problem 2 — Normal Distribution

Simulate 100,000 samples of size 10 from N(0,1). Compare sample (ddof=1) and population (ddof=0) standard deviations.
Plot and explain differences as sample size increases.

Problem 3 — t-Tests & Type II Error (β)

For mean differences d ∈ {0, 0.1, …, 1.0}, simulate two-sample t-tests (n=100 per group, α=0.05).
Estimate β (non-rejection rate) and plot β vs d. Discuss power and implications.

Problem 4 — ANOVA vs Multiple t-Tests

Generate three groups (n=30) with means 0, 0.5, and 1. Compare results from ANOVA and individual t-tests, and explain why ANOVA is preferred when comparing more than two means.

---
Referencing & Documentation

Citations are included inline near relevant code or text.
Commonly referenced documentation includes:

- [NumPy Random Generator](https://numpy.org/doc/stable/reference/random/index.html)
- [scipy.stats.f_oneway](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.f_oneway.html)
- [Type I & II Errors — Wikipedia](https://en.wikipedia.org/wiki/Type_I_and_type_II_errors)

---

Acknowledgements:

ATU course materials and Ian McLoughlin lecturer guidance.

Python libraries: NumPy, SciPy, Pandas, Matplotlib, Statsmodels.

External documentation and statistical references as cited.

---
© 2025 Hugo Camacho Romero

---
