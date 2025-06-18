# 📊 Stock Portfolio Heatmap Analyzer using CNN

An AI-powered financial analysis tool that uses deep learning (CNN) to analyze correlation heatmaps of selected stock tickers and provide investment recommendations.

## 🚀 Overview

This project helps users visualize the relationship between different stocks using a **correlation heatmap**, then uses a trained **Convolutional Neural Network (CNN)** to analyze the heatmap and suggest whether it's a good time to invest or not.

It combines:
- 📉 Stock data from [Yahoo Finance](https://finance.yahoo.com)
- 📊 Correlation analysis and heatmap generation
- 🤖 Image-based classification using CNN
- 🌐 Interactive UI built with **Gradio** and optionally extendable to **Streamlit**

---

## 📌 Features

- 📈 **Fetch live stock data** from Yahoo Finance using custom ticker inputs and date ranges
- 🌡️ **Generate a correlation heatmap** showing how stocks relate
- 🧠 **CNN-based investment prediction model**
- 🎨 **Interactive web interface** for real-time analysis
- 🪙 **Displays current stock prices** of entered tickers
- 🧪 Easily test with multiple portfolios

---

## 🧠 How It Works

1. **User Input**: Stock tickers and date range
2. **Data Fetching**: Download historical adjusted close prices
3. **Correlation Matrix**: Compute pairwise Pearson correlation between stock returns
4. **Heatmap Generation**: Visualize correlation matrix as an image
5. **Prediction**: Pass the heatmap to a CNN model trained to identify patterns that suggest profitable investments
6. **Output**: 
   - 📌 Heatmap Image
   - 💬 Investment Recommendation: `✅ INVEST` or `❌ DO NOT INVEST`
   - 💵 Current stock prices

---

## 🧪 Sample Inputs

Use the following inputs for testing:
Tickers: INFY.NS, TCS.NS, RELIANCE.NS, HDFCBANK.NS
Start Date: 2023-01-01
End Date: 2024-01-01

Try entering financial crisis periods like:
Tickers: AIG, LEH, JPM, MS
Start Date: 2007-01-01
End Date: 2009-01-01

---

## 🔧 Requirements

Install the required libraries:

pip install yfinance seaborn matplotlib tensorflow gradio pandas

---

▶️ Running the App
For Gradio:

bash
Copy
Edit
python app.py
For Google Colab:

Upload portfolio_cnn_model.h5 and run all cells

App will launch with public gradio.live link

---
✅ Future Improvements

🗂️ Save user sessions and prediction history
🔁 Rolling window dataset creation
🧮 Multiple ML models to compare
📊 Display additional financial indicators
🛠️ Portfolio optimization suggestions

---

📚 License
This project is under the MIT License.



