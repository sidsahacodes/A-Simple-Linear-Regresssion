# A Simple Linear Regression

This repository contains a Jupyter notebook that implements and analyzes a linear regression model using the prostate cancer dataset. The project emphasizes both the **theoretical foundations of Ordinary Least Squares (OLS)** and a **manual implementation of estimation, inference, and validation**, avoiding black-box regression libraries where possible.

## File Overview

- **`simple_LR.ipynb`**  
  Main analysis notebook. Covers model specification, estimation, assumption checks, statistical inference, and out-of-sample evaluation.

- **`prostate.csv`**  
  Dataset containing clinical and pathological measurements related to prostate cancer.

## Dataset Description

The dataset includes the following variables:

- **`lpsa`**: Log prostate-specific antigen (response variable)
- **`lcavol`**: Log cancer volume  
- **`lweight`**: Log prostate weight  
- **`age`**: Age of the patient  
- **`lbph`**: Log amount of benign prostatic hyperplasia  
- **`svi`**: Seminal vesicle invasion indicator (0 = no, 1 = yes)  
- **`lcp`**: Log capsular penetration  
- **`gleason`**: Gleason score  
- **`pgg45`**: Percentage of Gleason scores 4 or 5  

## Methodology

The notebook walks through the full OLS workflow:

1. **Model specification**
   - Linear regression with an intercept
2. **Manual OLS estimation**
   - Closed-form solution $(X^\top X)^{-1} X^\top y$
3. **Assumption checks**
   - Linearity
   - Multicollinearity
   - Homoskedasticity
4. **Statistical inference**
   - Estimation of error variance
   - Variance–covariance matrix
   - Standard errors
   - t-statistics and p-values
5. **Out-of-sample evaluation**
   - Train/test split
   - MSE, RMSE, and out-of-sample $R^2$
   - Actual vs. predicted plots

## Key Takeaways

- Tumor volume and prostate size emerge as the strongest predictors of PSA levels.
- Classical OLS assumptions are assessed explicitly rather than assumed.
- Out-of-sample performance is evaluated relative to a mean-prediction baseline.
- The project highlights the connection between estimation, inference, and prediction.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/sidsahacodes/A-Simple-Linear-Regresssion.git
