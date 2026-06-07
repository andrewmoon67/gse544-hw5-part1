# GSE 544 — Homework 5, Part 1

**Fitting Marginals and Copulas to the VMLS Portfolio**

**claude.ai and the 544_Notebooks were used to assist this homewokr**

## Contents

| File | Description |
|------|-------------|
| `hw5_part1.ipynb` | Main notebook — all five parts |
| `vmls_portfolio_returns.csv` | Input data (2000 training rows × 19 assets) |
| `figures/` | Auto-generated plots saved by the notebook |
| `requirements.txt` | Python dependencies |

## Setup

```bash
# 1. Clone the repo
git clone https://github.com/<your-username>/gse544-hw5.git
cd gse544-hw5

# 2. Create and activate a virtual environment (recommended)
python3 -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Launch Jupyter
jupyter notebook hw5_part1.ipynb
```

## Running the Notebook

Run all cells top-to-bottom (`Kernel → Restart & Run All`).  
The notebook will:
1. Load `vmls_portfolio_returns.csv` from the same directory
2. Save all figures to `figures/`
3. Print parameter tables and corner-mass statistics inline

## Structure

- **Part (a):** Student-t marginal fits for all 19 assets; summary for stocks 1, 2, 3, 10
- **Part (b):** Probability Integral Transform + 4×4 empirical scatter matrix
- **Part (c):** Gaussian copula fit (4×4 correlation matrix)
- **Part (d):** t-copula fit via profile MLE (correlation + ν̂)
- **Part (e):** Simulate n=2000 from each copula; compare corner mass
