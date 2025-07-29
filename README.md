# Shoppers-Spectrum
Customer Segmentation + Product Recommender app using RFM, KMeans, and Cosine Similarity — powered by Streamlit.
# 🛍️ Shopper Spectrum - Customer Segmentation and Product Recommender

This project combines **Customer Segmentation** using RFM analysis with a **Collaborative Filtering-based Product Recommendation System**, all integrated into a user-friendly **Streamlit web app**.

---

## 📌 Problem Statement

Businesses want to:
- Understand **shopper behavior**
- Target the right customer segments
- Recommend relevant products

This app solves that using:
- RFM-based segmentation (Recency, Frequency, Monetary)
- KMeans & Hierarchical clustering
- Product recommendations using cosine similarity

---

## 🚀 Features

### 👤 Customer Segment Prediction
- Enter Recency, Frequency, Monetary values
- Get segment labels like:
  - High Value
  - Loyal Whales
  - At-Risk
  - Low Value
  - Top VIPs

### 🧠 Product Recommender
- Enter any product name
- See the **top 5 most similar products** (based on cosine similarity)

---

## 🛠️ Technologies Used

| Component         | Tool/Library        |
|------------------|---------------------|
| Language         | Python              |
| Web Framework    | Streamlit           |
| Clustering       | KMeans, Hierarchical|
| Recommendation   | Cosine Similarity   |
| Data Handling    | pandas, scikit-learn|
| Model Saving     | joblib              |

---

## 📂 Project Structure
shopper_spectrum_app/
├── app.py # Streamlit application
├── scaler_rfm.pkl # StandardScaler for RFM
├── kmeans_rfm_model.pkl # Trained KMeans model
├── similarity_matrix.pkl # Cosine similarity matrix (products)
├── product_lookup.pkl # Dictionary: StockCode → Product Name
├── README.md # (This file)

---

## 💻 How to Run the App Locally

### 📌 1. Install Dependencies
pip install streamlit pandas scikit-learn joblib
**Launch the App**
streamlit run app.py
The app will open in your browser at:
http://localhost:8501
Note: **Do not close the terminal** while the app is running.
Segmentation Model Overview
RFM features were scaled and clustered using KMeans:
1. Recency: Days since last purchase.
2. Frequency: Number of purchases.
3. Monetary: Total money spent
Elbow and silhouette methods were used to determine the optimal number of clusters.

## 📸 App Screenshots

### 🔹 Product Recommender
![Product Recommender](https://1drv.ms/i/c/d0b10f70d6327ec1/Ed7ctriqm9BGpMKtmHW3ZYIBLkWf_bDT7nOlKeq_q_FbQw?e=ntgMfo)

### 🔹 Customer Segment Predictor
![Customer Segment](https://1drv.ms/i/c/d0b10f70d6327ec1/EXb3LXGxlTBJi2Oem-QtYgABBbcOMhZbho1Wy-Pt6MyMBw?e=DbQW0O)

Author
Shailesh Jangam
Data Science Enthusiast | https://www.linkedin.com/in/shailesh-jangam
Email: shaileshjangam79@gmail.com
