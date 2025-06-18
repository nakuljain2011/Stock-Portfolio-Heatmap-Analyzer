# Stock-Portfolio-Heatmap-Analyzer

This project builds a Convolutional Neural Network (CNN) model that classifies stock correlation heatmaps to help automate financial portfolio allocation decisions. It uses historical stock price data to generate heatmaps of correlations between selected assets, and trains a deep learning model to make binary predictions based on these visual patterns.

---

## 🚀 Features

- ✅ Fetch historical stock data using `yfinance`
- 📈 Generate correlation matrices and heatmaps
- 🧠 Train a CNN model to classify the heatmaps
- 🔮 Predict labels for new heatmaps using the trained model
- 📁 Organized folder structure for image storage and labels
- 🧪 Includes dummy dataset generation for testing/training

---

## 📦 Requirements

Install dependencies using:

```bash
pip install yfinance numpy pandas seaborn matplotlib tensorflow scikit-learn

🛠️ How It Works
Data Fetching
Fetch stock prices using yfinance for a selected date range.

Heatmap Generation
Compute the correlation matrix from daily returns and visualize it using seaborn.

Model Training
A CNN is trained using image inputs of the heatmaps and synthetic labels.

Prediction
The trained CNN can predict labels for new or unseen heatmap images.
