# 🧠 GPUlytics: Predictive Analysis of GPU Giants (NVIDIA, AMD, Intel)

A time-series deep learning project that forecasts stock prices of GPU market leaders by leveraging historical trends, trading volume, and AI-powered modeling. Built for data-driven investment insights in a rapidly evolving AI and GPU-driven world.

## 📊 Project Overview

**GPUlytics** is a predictive analytics project focused on forecasting the stock prices of **NVIDIA**, **AMD**, and **Intel** using advanced machine learning models like **LSTM Neural Networks**. The project combines historical stock data, trading volume patterns, and investor behavior insights to deliver accurate and timely price predictions.

> 📅 Project Duration: March 2025  
> 🧑‍🎓 Author: Meet Desai  
> 🏫 Program: MS in Data Science @ Pace University  
> 🧪 Course: Practical Data Science  

## 🔍 Problem Statement

GPU industry stocks are increasingly volatile due to rapid shifts in AI adoption, macroeconomic changes, and investor sentiment. Traditional analysis methods struggle to capture these dynamics in real time.

## 💡 Proposed Solution

The solution integrates:

- ✅ 10-Year Historical Stock Prices (2015–2025)
- ✅ Trading Volume Trends
- ✅ LSTM Neural Network for sequential forecasting
- ✅ Volume as Sentiment Proxy to enhance prediction accuracy

## 🧾 Data Description

| Feature         | Description                                     |
|-----------------|-------------------------------------------------|
| `Date`          | Trading day date                                |
| `Open`          | Opening stock price                             |
| `High`          | Day's highest stock price                       |
| `Low`           | Day's lowest stock price                        |
| `Close`         | End-of-day stock price (prediction target)      |
| `Volume`        | Total shares traded (used for sentiment signal) |

- ⏱ Timeframe: March 24, 2015 – March 21, 2025  
- 📈 Source: Nasdaq Historical Quotes  
- 🧪 2515 Trading Days per Company

## 🔬 Exploratory Data Analysis Highlights

- 📈 NVIDIA surged post-2023, aligning with the global AI boom.
- 📊 AMD spiked between 2018–2023, reflecting aggressive innovation.
- ⚖️ Intel showed flat performance, indicating slower tech adaptation.
- 📉 High trading volume often preceded price jumps, especially for NVIDIA.
- 🔁 Cross-company correlations revealed shared market sentiment.

## 🧠 Modeling Approach

### LSTM Neural Network Architecture

- Input: Last 60 days of `Close` + `Volume`
- Framework: TensorFlow/Keras
- Layers:
  - LSTM(60) → Dropout(30%) → LSTM(60) → Dense(1)
- Optimizer: Adam
- Loss: Mean Squared Error
- Epochs: 15 | Batch Size: 32

📌 **Why LSTM?**  
LSTM captures temporal dependencies and memory across time — ideal for stock trends.

📌 **Volume Added?**  
Yes! Volume captures investor sentiment, improving predictions significantly.

## 📈 Key Findings

- 📊 Volume integration improved prediction accuracy across volatile periods.
- 🔮 LSTM captured bullish momentum effectively, especially for AMD and NVIDIA.
- ❗ Intel’s weak price-volume correlation affected model accuracy.

## 💼 Business Recommendations

1. **Integrate Enhanced LSTM Model**  
   Deploy the model in investment dashboards to optimize AI product launch timing and investment strategies.

2. **Use Volume Spikes as Early Signals**  
   Create real-time alerts to flag bullish/bearish sentiment — enabling faster executive decisions.

## 🛠 Technical Next Steps

- 🧠 Incorporate NLP sentiment analysis from news & earnings reports
- 📉 Integrate macroeconomic indicators (interest rates, inflation)
- 🔗 Build multi-stock multivariate models to capture market-wide sentiment
- 🔁 Experiment with Transformer-based architectures (e.g., Temporal Fusion Transformers)

## 📁 Project Structure

```
📦GPUlytics-Stock-Prediction-Model/
 ┣ 📂Datasets/
 ┃ ┣ 📄nvidia.csv
 ┃ ┣ 📄amd.csv
 ┃ ┗ 📄intel.csv
 ┣ 📄GPUlytics_Predictive_Analysis_of_GPU_Giants.ipynb
 ┣ 📄README.md
 ┣ 📄requirements.txt
```

## 🔗 Repository & Dataset Access

- **GitHub Repo:**  
  [https://github.com/MeetDesaii/GPUlytics-Stock-Prediction-Model](https://github.com/MeetDesaii/GPUlytics-Stock-Prediction-Model)

- **Datasets Folder:**  
  [Datasets Directory](https://github.com/MeetDesaii/GPUlytics-Stock-Prediction-Model/tree/main/Datasets)
  

## 🙌 Acknowledgements

Thanks to **Pace University**, Seidenberg School of Computer Science, and to **Stephanie Langeland - the faculty of Practical Data Science** for guidance and support.
