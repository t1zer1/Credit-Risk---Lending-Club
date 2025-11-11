# Credit Risk Default Prediction (Lending Club)

Predicting loan default probability on a 2007–2015 Lending Club–style dataset.  
This repository shows a full, reproducible ML workflow—from data prep and EDA to model benchmarking and evaluation.

---

## 🔎 Problem
Given borrower and loan attributes, estimate the probability a loan will **default**.  
This supports better risk-based decisions (pricing, approvals, limits) and model explainability for stakeholders.

---

## 📦 Models Benchmarked
- **Logistic Regression** — interpretable baseline
- **Decision Tree (no CV)** — simple, high variance
- **Decision Tree (CV-tuned)** — better bias/variance balance
- **Random Forest** — robust ensemble

### 📈 Headline Test Results
| Model | ROC-AUC (test) | Notes |
|---|---:|---|
| Decision Tree (CV-tuned) | ~0.84 | Best balance of accuracy & interpretability |
| Random Forest | ~0.83 | Strong generalisation, less transparent |
| Logistic Regression | ~0.76 | Reliable, easy to explain |
| Decision Tree (no CV) | ~0.64 | Overfits without tuning |

> Full write-up, figures and confusion matrices: **`report/credit_risk_analysis_report.pdf`**  
> Reproduce the pipeline in **`notebooks/credit_risk_models.ipynb`**.

---

## 🗂 Repository Structure
