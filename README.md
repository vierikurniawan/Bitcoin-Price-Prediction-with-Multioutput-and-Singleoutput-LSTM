# 📈 Bitcoin Price Prediction with Multioutput and Singleoutput LSTM
This project focuses on predicting Bitcoin prices using Long Short-Term Memory (LSTM) neural networks. It implements two types of LSTM models:
- Multioutput LSTM: Predicts multiple future prices at once.
- Singleoutput LSTM: Predicts one future price at a time.
  
The goal is to analyze the effectiveness of different sequence lengths (SEQ_LEN) and compare prediction accuracy.

## 🚀 Project Overview
- 🔍 Goal: Predict future Bitcoin closing prices based on historical data using LSTM.
- 🗂 Dataset: [Bitcoin historical close price data from 2014-09-17 until 2023-12-09](https://coinmarketcap.com/currencies/bitcoin/historical-data/).
- 🏗 Approach: Data preprocessing, feature scaling, sequence generation, LSTM model training & evaluation.
- 🎯 Evaluation Metric: Mean Absolute Percentage Error (MAPE).
- 🔄 Comparisons: Multioutput vs. Singleoutput LSTM models with different sequence lengths.

## 🛠 Tech Stack
- Programming Language: Python
- Libraries:
  - Machine Learning & Deep Learning: TensorFlow, Keras, Scikit-learn
  - Data Processing: Pandas, NumPy
  - Visualization: Matplotlib
 
## 📊 Results
The models are evaluated using MAPE (Mean Absolute Percentage Error):

Model	Sequence Length	Prediction Length	MAPE (%)
- Multioutput LSTM	with 150-day sequence used to predict the next	30 days:	42.57%
- Singleoutput LSTM	with 150-day sequence used to predict 1 future price:	5.98%

On the other hand, the validation loss fluctuates significantly while the training loss remains low, indicating that the model might be overfitting.

## 📌 Key Insights
- Multioutput LSTM allows for the prediction of multiple future prices but may have higher error rates.
- Singleoutput LSTM is more focused but requires iterative predictions for long-term forecasting.

## 🏗 How to Run
1️⃣ Clone this repository
```bash
git clone https://github.com/vierikurniawan/Bitcoin-Price-Prediction-with-Multioutput-and-Singleoutput-LSTM.git  
cd Bitcoin-Price-Prediction-with-Multioutput-and-Singleoutput-LSTM  
```
2️⃣ Install dependencies
```bash
pip install numpy pandas tensorflow scikit-learn matplotlib
```  
3️⃣ Run the Script
```bash
python Bitcoin_Price_Prediction_with_LSTM.ipynb
```
