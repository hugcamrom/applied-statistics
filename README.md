# [**Applied Statistics**](https://en.wikipedia.org/wiki/Statistics#Applied_statistics,_theoretical_statistics_and_mathematical_statistics)

<!--Study of the practical use of statistical methods to collect, analyse, interpret, and present data in real-world contexts.-->

![mindtouchbyappliedstats](images/libretextsorg2025-12-07.jpg)

[![Python](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Notebook-Jupyter-orange.svg)](https://jupyter.org/)

---

This repository contains my official submission for the **Applied Statistics** assessment.  
It is structured, documented, and reproducible — providing a clear demonstration of statistical understanding and computational implementation.

All finalised solutions and explanations are contained within the main notebook:  
**[`problems.ipynb`](./problems.ipynb)**  

---

## Overview & Purpose

The [**Applied Statistics**](https://atu.ie) module enables students to demonstrate their ability to:

1. **Describe** the stochastic nature of real-world measurements.  
2. **Source documentation** to programmatically perform a statistical test.  
3. **Select** the appropriate statistical test to investigate a claim.  
4. **Perform** a statistical test on a dataset and interpret the results.

---

## Development Environment — GitHub Codespaces (“improved telegram”)

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://docs.github.com/en/codespaces/quickstart)

This repository is hosted and developed in [**GitHub Codespaces**](https://docs.github.com/en/codespaces/quickstart), under the workspace named **“improved telegram”**.

By default, a Codespace development environment runs on a **virtual machine (VM)** based on [**Ubuntu Linux**](https://en.wikipedia.org/wiki/Ubuntu#:~:text=Ubuntu%20can%20be%20installed%20directly,for%20platforms%20such%20as%20OpenStack.) and includes many popular tools and languages.  
This setup ensures a consistent, cloud-based environment regardless of your local operating system.

**Key features:**

- Runs entirely in a **Linux (Ubuntu)** environment.  
- Compatible with **Python, Jupyter, [Git](https://git-scm.com/), and command-line utilities** preinstalled.  
- You can extend or customise the base image with additional libraries or tools.  
- Windows and macOS are *not* supported as remote container OS options — all Codespaces execute within Linux.  
- Ideal for running notebooks, simulations, and data visualisations directly in the browser.

This ensures consistent behaviour for numerical computing and plotting across devices and operating systems.

---

## Repository Structure

```bash
├── README.md             # This file — overview, purpose, and guidance
├── problems.ipynb        # Main notebook with all solutions (assessment focus)
├── requirements.txt      # Minimal reproducible environment
├── .gitignore            # Python + Jupyter configuration
└── images/               # (Optional) saved figures used in the README/notebook
```

---
## Requirements

The assessment requires a minimal reproducible environment, provided in **[`requirements.txt`](./requirements.txt)**.

The final notebook uses:

- [NumPy](https://numpy.org/) — numerical computing
- [SciPy](https://scipy.org/) — statistical tests (t‑tests, ANOVA, Tukey HSD)
- [Pandas](https://pandas.pydata.org/) — organising results in tables
- [Matplotlib](https://matplotlib.org/) — plots and visualisation
- [IPython](https://ipython.org/) — notebook runtime support

During development, additional libraries may be available in Codespaces, but they are **not required** for running the submitted notebook.

---
## How to run

### Option 1 — Local

```bash
git clone https://github.com/hugcamrom/applied-statistics.git
cd applied-statistics
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

Open **`problems.ipynb`** and run the notebook from top to bottom.

### Option 2 — GitHub Codespaces

Open the repository on GitHub and choose **Code → Create codespace on main**.
Then open **`problems.ipynb`** and run all cells.

---

## Notebook structure and problem summary

All work is presented in a single notebook: **[`problems.ipynb`](./problems.ipynb)**.

Each problem includes:

- **Plan & references** (Markdown)
- **Implementation** (well‑commented Python code)
- **Plots & tables** (clear, labelled outputs)
- **Interpretation** (concise explanation of results)

### Problem 1 — Extending the Lady Tasting Tea

- Compute and simulate the probability of correctly identifying all cups by chance for:
  - the classic 8‑cup design (4 tea‑first vs 4 milk‑first), and
  - an extended 12‑cup design (8 tea‑first vs 4 milk‑first).
- Compare exact vs simulated probabilities and discuss implications for p‑value thresholds.

### Problem 2 — Normal distribution (sample vs population standard deviation)

- Generate 100,000 samples of size 10 from a standard normal distribution.
- Compute the standard deviation using:
  - `ddof=1` (sample SD), and
  - `ddof=0` (population SD).
- Plot both distributions and discuss how differences change as sample size increases.

### Problem 3 — t‑tests and Type II error (β)

- For mean differences \( d \in \{0, 0.1, \dots, 1.0\} \), run 1,000 simulations per value:
  - draw two samples (n=100 each),
  - run an independent two‑sample t‑test (α = 0.05),
  - estimate the Type II error rate \( \beta(d) \) as the proportion of non‑rejections.
- Plot \( \beta(d) \) against \( d \) and interpret how power increases with effect size.

### Problem 4 — ANOVA vs multiple t‑tests (with Tukey HSD)

- Generate three groups (n=30 each) from normal distributions with means 0, 0.5, and 1.
- Compare:
  - one‑way ANOVA,
  - three pairwise two‑sample t‑tests,
  - Tukey’s HSD post‑hoc comparisons.
- Explain why ANOVA is preferred when comparing more than two means.

---

## Referencing

References are included inline near the relevant code or explanation. Commonly used sources include:

- [NumPy Random Generator](https://numpy.org/doc/stable/reference/random/index.html)
- [scipy.stats.f_oneway](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.f_oneway.html)
- [Type I & II Errors — Wikipedia](https://en.wikipedia.org/wiki/Type_I_and_type_II_errors)

---

## Getting Help & AI Usage

During development, I used AI tools (including VSC GitHub Copilot and ChatGPT) as a support for drafting text, refining explanations, and reviewing code, not as an automatic solution generator.

All code, simulations, and interpretations were manually checked for correctness and clarity. The final responsibility for this submission lies with me as the student.

---

## Acknowledgements

ATU course materials and Ian McLoughlin lecturer guidance.

Python libraries: NumPy, SciPy, Pandas, Matplotlib.

External documentation and statistical references as cited.

Image credit: Pixabay (ID 2062057) – Pixabay Content License.

---

© 2025 Hugo Camacho Romero

---
