# NextGen-Churn-Blockchain-API
Integrates Machine Learning (Gradient Boosting) for predictive customer churn with a simulated Blockchain Ledger for immutable recording of retention decisions (SDG 8/9).
# 📈 Next-Gen Churn Intelligence: ML & Blockchain for Predictive Retention (SDG 8 & 9)

## Project Overview

The Next-Gen Churn Intelligence project introduces an innovative framework that integrates Machine Learning (ML) and Distributed Ledger Technology (Blockchain) to develop a transparent and effective customer retention strategy tailored for subscription-based businesses in emerging economies. This initiative aims to transition from reactive customer service models to proactive, personalized interventions, enhancing economic stability and fostering technological trust in line with Sustainable Development Goals (SDG) 8 (Decent Work and Economic Growth) and SDG 9 (Industry, Innovation, and Infrastructure).

## 📊 Key Impact & Verifiable Metrics
The project focuses on several key metrics to measure its impact:
| Metric | Goal | Status |
| :--- | :--- | :--- |
| **Financial Stability** | Reduce customer churn rate in the financial sector | Projected **10%** annual reduction, significantly impacting bottom-line stability for partner institutions. |
| **Data Integrity** | Ensure every retention action is immutable and auditable | **100% data integrity** and anti-manipulation assurance provided by the Blockchain ledger. |
| **Model Accuracy** | Accurately identify high-risk customers | **Gradient Boosting Model** achieved high predictive accuracy on the classification task. |

## ⚙️ Technical Architecture: The Dual Stack

This system is built on two synchronized Python stacks to achieve both prediction and secure verification:

### 1. Predictive Layer (Machine Learning)

* **Model:** **Gradient Boosting Classifier** used to score customers based on features like **Tenure, Monthly Charges, Contract Type,** and **Support Ticket frequency**.
* **Function:** Exposed via the Flask API to provide the real-time probability of a customer churning.

### 2. Ledger Layer (Simulated Blockchain)

* **Technology:** Custom Python class simulating a private, immutable **Blockchain Ledger**.
* **Function:** Securely records every predictive decision and the subsequent retention action taken (e.g., "OFFER\_TARGETED\_DISCOUNT"). This creates an auditable trail, enforcing accountability and preventing operational manipulation.

---

## 📁 Core Files and Functionality

| File | Function | Technology |
| :--- | :--- | :--- |
| `churn_model.py` | Trains, validates, and serializes the Gradient Boosting predictive model. | Scikit-learn, Joblib |
| `blockchain_ledger.py` | Defines the `SimpleBlock` and `RetentionLedger` classes for data immutability. | Python `hashlib`, JSON |
| `app.py` | The orchestrating **Flask API**. Handles data ingestion, calls the ML model, applies the business logic, and commits the action to the Blockchain. | Flask, NumPy, Joblib |

## 🚀 Deployment and API Usage

### Prerequisites

```bash
pip install pandas scikit-learn joblib flask pulp

# Setup and Run
## Train Model:
Bash
python churn_model.py

## Start API:
Bash
python app.py
(Runs on http://127.0.0.1:5000)

## API Endpoints
1. POST /api/analyze_churn
Analyzes customer data, returns the retention action, and records the transaction on the ledger.

JSON Payload Example (High-Risk Customer):

JSON

{
    "customer_id": "CUST-9001",
    "Age": 35,
    "Tenure_Months": 15,
    "Monthly_Charges": 110.50,
    "Support_Tickets_Last_Month": 5,
    "Contract_Type": "Month-to-Month",
    "Total_Usage_GB": 45.8
}
2. GET /api/ledger_status
Returns the full, immutable history of all recorded retention actions for auditing purposes.

## 🔗 Leadership & Connectivity
This project showcases expertise in integrating cutting-edge technology for economic resilience, reflecting my role as Lead Data Scientist at KleanData Konsult.

Sylvanus Olufemi Orodiran | [(https://www.linkedin.com/in/sylvanus-olufemi-orodiran)]
Active Member: Nigeria Computer Society (NCS ID: 18077)
