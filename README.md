# A Machine Learning-Driven Business Intelligence Framework for Predictive Supply Chain Risk Monitoring and Decision Support at Business Unit Level 
Overview
This project presents a comprehensive analytical framework for continuous international supply chain risk assessment using real-time, non-proprietary data sources. The system transforms raw global data into actionable intelligence to support proactive decision-making in volatile environments.

The solution integrates machine learning, anomaly detection, and economic indicators to identify risks arising from geopolitical instability, logistics disruptions, and unexpected global events.

Objectives
Develop a real-time supply chain risk monitoring system

Integrate structured economic data with unstructured event data

Detect sudden disruptions ("black swan" events)

Provide interpretable and actionable risk scores

Support compliance with regulatory frameworks (e.g., LkSG, CSRD)

Enable data-driven strategic decision-making

Methodology
1. Data Sources
World Bank Indicators → Governance, logistics, and economic metrics

GDELT Dataset → Global news and event intensity data

2. Machine Learning Model (Ensemble)
A stacked ensemble of:

Random Forest

LightGBM

XGBoost

CatBoost

These models process structured features such as governance indicators and logistics performance metrics.

3. Anomaly Detection System
To capture rare and high-impact events:

Isolation Forest

One-Class SVM

Local Outlier Factor (LOF)

HDBSCAN

This layer detects anomalies that traditional predictive models may miss.

4. Risk Scoring Engine
A composite risk score is generated using:

Model predictions

Event intensity signals

Structural economic indicators

5. Optimization Module
An "Upgrade Pack" optimizes alert thresholds for improved decision-making, achieving measurable performance gains.

Key Features
Real-time global risk monitoring

Hybrid ML + anomaly detection architecture

High interpretability with feature importance analysis

Scalable and modular pipeline

Compliance-ready outputs (audit-friendly documentation)

Repository Structure
├── Thesis.ipynb        # Main implementation notebook
├── data/               # (Optional) Input datasets
├── outputs/            # Generated results, visualizations
├── README.md           # Project documentation
Installation & Setup
1. Clone the repository
git clone https://github.com/your-username/supply-chain-risk.git
cd supply-chain-risk
2. Install dependencies
pip install -r requirements.txt
3. Run the notebook
jupyter notebook Thesis.ipynb
Results and Insights
Ensemble models outperform individual models in predictive accuracy

Governance indicators (e.g., WGI_MEAN) show high feature importance

Anomaly detection significantly improves early disruption detection

The system provides proactive insights without reliance on delayed reports

Use Cases
Global supply chain monitoring

Risk assessment for international sourcing

Regulatory compliance reporting

Strategic planning under uncertainty

Technologies Used
Python

Scikit-learn

LightGBM, XGBoost, CatBoost

Pandas, NumPy

Matplotlib / Seaborn

Future Work
Integration with live streaming APIs

Dashboard deployment (Power BI / Streamlit)

Incorporation of deep learning models

Enhanced explainability modules

Author
Add your name here

License
This project is for academic and research purposes.
