FraudShield
Explainable Fraud Detection in Online Transactions using Graph Neural Networks
📌 Overview

FraudShield is an end-to-end fraud detection system designed to identify suspicious online transactions by modeling transaction data as a graph and applying Graph Neural Networks (GNNs) to capture complex relational patterns between users, merchants, and transactions.

The system emphasizes explainability, using SHAP and LIME to make fraud predictions interpretable, and includes an interactive Streamlit dashboard for analysis and visualization.

🎯 Objective

Detect fraudulent transactions with higher accuracy than rule-based methods

Capture relational patterns that traditional ML models miss

Provide transparent and explainable predictions for trust and governance

Enable interactive exploration of fraud insights through a dashboard

🗂 Problem Statement

Traditional fraud detection systems often:

Treat transactions independently

Fail to capture relationships between users, devices, and merchants

Act as black boxes with limited explainability

FraudShield addresses these limitations using graph-based learning and model interpretability techniques.

🧠 Methodology
1️⃣ Data Representation as a Graph

Transactions modeled as a graph structure

Nodes represent:

Users

Merchants

Transactions

Edges represent:

Transaction relationships

Shared attributes (e.g., device, location)

This structure enables learning fraud patterns across connected entities.

2️⃣ Graph Neural Network (GNN)

Applied GNN models to:

Learn node embeddings

Capture neighborhood-level fraud behavior

The model identifies suspicious patterns such as:

Repeated transactions

Unusual connections

Fraud rings or clusters

3️⃣ Fraud Prediction

Each transaction is classified as:

Fraudulent

Non-fraudulent

Model outputs probability scores rather than hard decisions

4️⃣ Explainability (SHAP & LIME)

To ensure transparency:

SHAP used for global feature importance

LIME used for local, transaction-level explanations

This helps answer:

Why was this transaction flagged as fraud?

Which features influenced the decision most?

5️⃣ Interactive Dashboard (Streamlit)

Visualizes:

Fraud predictions

Explanation plots

Transaction-level insights

Allows users to explore:

Individual transactions

Model behavior

Risk drivers

✅ Current Project Status

✔ Graph-based data modeling
✔ GNN-based fraud detection
✔ Explainable AI using SHAP & LIME
✔ Interactive Streamlit dashboard

🚧 Future enhancements

Real-time streaming integration

Model performance benchmarking

Scalability improvements for large transaction graphs

🔍 Key Learnings

Graph representations significantly improve fraud detection accuracy

Explainability is essential for trust in financial ML systems

GNNs are well-suited for relational risk problems like fraud

🛠 Tech Stack

Python

PyTorch / PyTorch Geometric

NetworkX

Scikit-learn

SHAP, LIME

Streamlit

Pandas, NumPy

📁 Project Structure
FraudShield/
│
├── data/                 # Transaction datasets
├── graph/                # Graph construction logic
├── models/               # GNN models
├── explainability/       # SHAP & LIME analysis
├── dashboard/            # Streamlit app
└── README.md

📌 Use Case Relevance

This project demonstrates how graph-based ML and explainable AI can be applied to:

Financial crime prevention

Risk analytics

Decision support systems

The concepts align closely with enterprise risk platforms used in banking and fintech.

📎 Disclaimer

This project is for educational and research purposes.
It demonstrates fraud detection techniques and does not represent a production-grade financial system.
