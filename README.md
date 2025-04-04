# AI-Based-stock-prediction
This project leverages a lightweight Small Language Model (SML) architecture to predict short-term trends in stock prices. The system is designed to analyze historical financial text data and numerical stock prices to forecast future movements in the market with minimal computational resources.

Technical Details:
1. Data Collection & Preprocessing:
Sources: Historical stock price datasets (e.g., Yahoo Finance or Alpha Vantage), and financial news headlines.

Features Used:

Open, High, Low, Close (OHLC) prices

Volume

News sentiment scores (optional text data input for SML)

Preprocessing:

Normalization of numerical values (Min-Max scaling or Z-score)

Tokenization and embedding of text (if sentiment/news data used)

Time-series windowing for sequence prediction (e.g., 7-day input → 1-day prediction)

2. Model Architecture (SML):
Model Type: A distilled, lightweight transformer or LSTM-based SML

Layers:

Embedding/Input layer for time-series sequences

2–3 LSTM or transformer encoder layers

Dense (fully connected) output layer for regression or classification (Up/Down)

Optimizer: Adam

Loss Function: Mean Squared Error (MSE) for regression or Binary Crossentropy for classification

Framework: TensorFlow / PyTorch (depending on implementation)

3. Output:
Regression Mode: Predicts future stock price (e.g., next-day closing price)

Classification Mode: Predicts trend direction (Up/Down/Neutral)

4. Evaluation Metrics:
RMSE / MAE for regression

Accuracy, Precision, Recall, F1-Score for classification

Optional: Backtesting to compare predicted vs actual performance in a simulated trading environment

5. Deployment:
Deployed as a lightweight web app using Flask or Streamlit, allowing users to input ticker symbols and receive predictions in real-time.

Use Case:
Ideal for educational use or lightweight predictive tasks in fintech research, especially where computational efficiency and explainability are key.

