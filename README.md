# Cybersecurity Intrusion Detection System (IDS)

An end-to-end machine learning capstone project that detects network
intrusions using behavioral and session-level features, with a full
pipeline from data understanding through explainability and fairness
auditing.

## 📊 CAPSTONE Overview

- **Task:** Binary classification (attack vs. normal), with an
  unsupervised anomaly-detection supplement (Isolation Forest)
- **Dataset:** [Kaggle — Cybersecurity Intrusion Detection Dataset](https://www.kaggle.com/datasets/dnkumars/cybersecurity-intrusion-detection-dataset)
- **Best model:** *Decision Tree (F1-Score macro 0.7778)*

## 🗂️ Repository Structure
├── src/          |  # Notebook-based reusable functions (see src/README.md) |
├── notebooks/    | # Main capstone analysis notebook |
├── data/         | # Not committed — dataset auto-downloads via kagglehub |
├── models/       | # Saved model artefacts (final_model.pkl, scaler, config) |
├── reports/      |  # Generated CSV/text reports (audits, metrics, summaries) |
├── figures/      |  # Saved visualisations (PNG) |
├── docs/         | # Final report and presentation decks (technical + business) |
├── requirements.txt |
├── LICENSE       |  # MIT License |
└── README.md     |

## 🚀 Getting Started

1. Clone this repository:
```bash
   git clone https://github.com/raireyes58/Cybersecurity-Intrusion-Detection-System-CAPSTONE-.git
   cd Cybersecurity-Intrusion-Detection-System-CAPSTONE-
```

2. Install dependencies:
```bash
   pip install -r requirements.txt
```

3. Set up your Kaggle API key (required for automatic dataset download):
   - Follow instructions at https://www.kaggle.com/docs/api
   - Place `kaggle.json` at `~/.kaggle/kaggle.json`

4. Run the notebook:
```bash
   jupyter notebook notebooks/
```
   The dataset downloads automatically in Step 2.2 — no manual download needed.

## 📈 Pipeline Summary

| Step | Description |
|------|-------------|
| 1 | Problem Understanding & Framing |
| 2 | Data Collection & Understanding (dataset justification, audits, data dictionary) |
| 3 | Data Preprocessing, Applied EDA & Feature Engineering |
| 4 | Model Implementation (6 models compared, tuned, cross-validated) |
| 5 | Explainability (SHAP/PDP/ICE), Limitations & Bias/Fairness Auditing |
| 6 | Final Presentation (Technical + Business decks — see `docs/`) |
| 7 | This repository |

## 🔍 Key Results

- Best model: **Decision Tree**
- F1-Score (macro): **0.7778*
- Recall (attack detection): **0.7749**
- ROC-AUC: **0.7942**

## ⚖️ Responsible AI

This project includes a bias and fairness audit (Step 5.5–5.7) using proxy
attributes (e.g. IP reputation), since the dataset contains no direct
demographic fields. See `reports/step5_8_bias_fairness_analysis_report.txt`
for the full analysis, including fairness metrics (demographic parity,
equalized odds, disparate impact) and mitigation recommendations.

## 📄 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.

## 👤 Author

- **Raizza Reyes-Basa**
- **Postgrad Diploma in Artificial Intelligence and Machine Learning**
- **Asian Institute of Management**
- **Class of 2025 - COHORT 3**
- **Linkedin : https://www.linkedin.com/in/raireyes/**


