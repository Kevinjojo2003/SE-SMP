# Sentiment-Enhanced Stock Market Predictor (SE-SMP)

## Overview

Sentiment-Enhanced Stock Market Predictor (SE-SMP) is an advanced multi-modal deep learning framework designed to predict stock market prices by integrating:
- Historical stock data
- Sentiment analysis of news articles
- Technical chart analysis using computer vision techniques

## Features

- 🔍 **Comprehensive Data Collection**
  - Retrieves historical stock data using yfinance API
  - Aggregates news articles and sentiment scores via News API

- 🧠 **Advanced Machine Learning**
  - LSTM neural networks for time-series forecasting
  - Ensemble methods using Random Forest, Gradient Boosting, and XGBoost
  - Hyperparameter tuning for model optimization

- 📊 **Sophisticated Analysis**
  - Technical indicator generation (SMA, EMA, RSI, MACD)
  - Sentiment-based feature engineering
  - Computer vision-based chart pattern recognition

- 🌐 **Real-Time Predictions**
  - Continuous stock price and sentiment analysis
  - Live data integration
  - Automated prediction updates

- 🖥️ **Interactive Streamlit Dashboard**
  - User-friendly interface
  - Real-time visualizations
  - Prediction and sentiment insights

## Prerequisites

- Python 3.7+
- Dependencies listed in `requirements.txt`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/SE-SMP.git
   cd SE-SMP
   ```

2. Create and activate a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Run Streamlit Dashboard
```bash
streamlit run app.py
```

### Manual Data Collection and Preprocessing
```bash
python data_collection.py
python preprocessing.py
```

### Model Training
```bash
python hyperparametertuning.py
```

## Project Structure
```
SE-SMP/
├── app.py                      # Streamlit dashboard
├── data_collection.py          # Stock and news data collection
├── preprocessing.py            # Data preprocessing
├── hyperparametertuning.py     # Model training and tuning
├── lstm_model.py               # LSTM model
├── real_time_chart_analysis.py # Computer vision chart analysis
├── feature_engineering.py      # Feature creation
├── ensemble.py                 # Ensemble learning
├── requirements.txt            # Dependencies
├── eda_outputs/                # EDA visualization directory
└── models/                     # Trained model storage
```

## Key Technologies

- Machine Learning: LSTM, Random Forest, XGBoost
- Data Processing: Pandas, NumPy
- Sentiment Analysis: NLP techniques
- Computer Vision: OpenCV
- Web Framework: Streamlit
- APIs: yfinance, News API

## Testing

Validate system performance through:
- Data collection accuracy
- Model performance metrics (MAE, MSE)
- Real-time prediction reliability

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

 MIT License

## Disclaimer

Stock market predictions are inherently uncertain. This tool is for educational and research purposes and should not be considered financial advice.
