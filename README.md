# 🏡 Azure ML Housing Price Prediction (End-to-End)

## 🚀 Project Overview

This project demonstrates an **end to end Machine Learning solution on Microsoft Azure**, from data ingestion to real-time model deployment.

As a **Technical Project Manager**, I built this to bridge the gap between:

* AI/ML theory
* Real-world cloud delivery challenges

---

## 🎯 Business Problem

Real estate stakeholders need accurate property price predictions to:

* Improve pricing strategies
* Reduce investment risk
* Enable data-driven decisions

---

## 🧠 Solution Architecture

![Architecture](architecture/architecture-diagram.png)

Pipeline:

1. Data ingestion from Azure Blob Storage
2. Dataset registration in Azure ML
3. AutoML regression experiment
4. Model selection (based on RMSE)
5. Real-time endpoint deployment
6. API consumption via Python

---

## ⚙️ Tech Stack

* Azure Machine Learning
* AutoML (Regression)
* LightGBM, XGBoost, ElasticNet
* Azure Blob Storage
* REST API
* Python (Jupyter Notebook)

---

## 📊 Model Details

* Task: Regression
* Target: Housing Price
* Metric: Normalized RMSE
* Best Model: LightGBM (AutoML selected)

---

## 🚀 Deployment

* Real-time endpoint deployed on Azure
* VM: Standard_D2a_v4
* REST API used for live predictions

---

## 🔗 API Example

```python
import requests

url = "YOUR_ENDPOINT_URL"
headers = {"Authorization": "Bearer YOUR_KEY"}

data = {
    "data": [
        {
            "sqft": 2000,
            "bedrooms": 3,
            "location": "urban"
        }
    ]
}

response = requests.post(url, json=data, headers=headers)
print(response.json())
```

---

## 📸 Screenshots

### AutoML Run

![AutoML](screenshots/automl-run.png)

### Endpoint Deployment

![Endpoint](screenshots/endpoint.png)

---

## 💡 Key Learnings (PM Perspective)

* 💰 Cost governance in cloud ML is critical
* ⚠️ Quota & region issues = delivery risks
* 🚀 Deployment is harder than training
* 🔄 DS → Engineering handoff requires strong ownership

---

## 🧹 Cost Optimization

* Decommissioned resource group after testing
* Avoided unnecessary compute charges

---

## 📁 Documentation

Full project walkthrough available here:
📄 docs/project-walkthrough.pdf

---

## 👤 About Me

Jaswant Singh
Technical Project Manager | AI & Cloud Enthusiast

Open to:

* Senior TPM roles
* AI/ML Delivery roles

---
