# 📈 Stock Price Predictor using LSTM (Interactive)

A time-series forecasting project that predicts stock prices using an LSTM (Long Short-Term Memory) deep learning model. Built in Google Colab, this project allows you to select a stock (e.g., AAPL, GOOG, etc.) and predict the closing price for the next 7 days.

---

## 🚀 Features

- 🔍 Load and explore real or custom historical stock data
- 📊 Visualize actual vs. predicted prices
- 🤖 Train an LSTM model on each stock dynamically
- 📅 Predict prices for the next 7 days
- 💾 Save predictions to CSV
- 🎛️ Interactive UI using ipywidgets (dropdown + button)

---

## 📁 Files

| File | Description |
|------|-------------|
| Stock_Market_Prediction_CLEANED.ipynb | Clean Colab notebook with LSTM prediction, dropdown UI, and CSV export |
| Stock_Price_Dataset.csv | Stock price dataset containing historical data for multiple companies |
| *.csv | Auto-generated 7-day forecast for each stock you run the model on |

---

## 📦 Requirements

Google Colab takes care of most dependencies, but in case you're running locally:

bash
pip install yfinance seaborn scikit-learn keras ipywidgets matplotlib
📊 How It Works
Load and clean the dataset (Date, Ticker, Open, Price, Risk).

Use ipywidgets.Dropdown to select a stock from the dataset.

Train an LSTM model using 95% of the stock’s historical data.

Predict the next 7 days using the last 60 days of stock prices.

Visualize the forecast and export predictions to a CSV file.

🧪 Model Architecture
2 stacked LSTM layers (50 units each)

Dense layer with 25 neurons

Final Dense output layer (1 neuron)

Optimizer: Adam

Loss: Mean Squared Error


📂 Example Prediction Output (CSV)
Date,Predicted_Price
2025-07-13,184.21
2025-07-14,185.33
2025-07-15,186.15
...
👨‍💻 Author
Tanishq Tiwari
📬 txnishq28

⭐️ Star This Repo
If you found this helpful, please give the project a ⭐ on GitHub! It helps others discover it too!


Would you like me to:
- Add this to your repo directly?
- Include setup instructions for Streamlit or Gradio version?

Let me know and I can customize further
