# 🛒 Graph-Based Product Recommendation Engine

An intelligent **product recommendation system** that uses **graph theory and community detection** to discover relationships between products based on customer purchasing behavior.

The system builds a weighted product network, detects product communities using the **Louvain algorithm**, and provides recommendations via a **Flask web application**.

---

## 📌 Project Overview

This project analyzes e-commerce transaction data to:

- Model customer–product relationships as graphs
- Identify product communities using clustering
- Generate personalized product recommendations
- Deploy recommendations using a web interface

Dataset used: **Online Retail Dataset (UCI)**

---

## 🚀 Features

- Customer–Product bipartite graph modeling  
- Product–Product weighted interaction network  
- Louvain community detection for product clustering  
- Graph visualization using NetworkX & Matplotlib  
- Recommendation engine based on normalized co-purchase probability  
- Model export to CSV for deployment  
- Flask-based web application for real-time recommendations  

---

## 🧠 Recommendation Approach

1. Build customer–product purchase matrix  
2. Convert to binary interaction matrix  
3. Compute product co-purchase frequency  
4. Normalize interaction strength  
5. Construct weighted product graph  
6. Detect communities (Louvain)  
7. Generate top-N recommendations  
8. Serve results via Flask UI  

---

## 🛠️ Technologies Used

- Python 3  
- Pandas, NumPy  
- NetworkX  
- Matplotlib  
- python-louvain (community detection)  
- Flask + Flask-CORS  
- Gephi (optional visualization)  

---

## 📂 Folder Structure

```text
graph-based-product-recommendation-engine/
│
├── data/
│   └── Online Retail.xlsx
│
├── model_training/
│   ├── preprocessing.py
│   ├── graph_builder.py
│   ├── louvain_clustering.py
│   └── recommendation_engine.py
│
├── products_prob.csv
│
├── web_app/
│   ├── app.py
│   ├── templates/
│   │   ├── index.html
│   │   └── about.html
│   └── static/
│
├── products.gexf
├── requirements.txt
└── README.md
