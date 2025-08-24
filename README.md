# IBM Stock Price Prediction using LSTM Neural Networks

A deep learning project that uses Long Short-Term Memory (LSTM) neural networks to predict IBM stock prices based on historical data. Built with PyTorch and integrated with Alpha Vantage API for real-time financial data.

## 🎯 Project Overview

This project demonstrates the application of deep learning techniques to financial time series forecasting. The model analyzes 25+ years of IBM stock price history to learn patterns and predict future closing prices.

## 🚀 Features

- **Deep Learning Architecture**: LSTM neural network with 2 layers and dropout regularization
- **Real-time Data**: Integration with Alpha Vantage API for live stock market data
- **Comprehensive Visualization**: Multiple charts showing training progress and predictions
- **Data Processing Pipeline**: Automated data normalization and sequence generation
- **Model Evaluation**: Visual comparison between actual and predicted prices

## 🛠️ Technology Stack

- **Python 3.x** - Core programming language
- **PyTorch** - Deep learning framework
- **NumPy** - Numerical computations
- **Matplotlib** - Data visualization
- **Alpha Vantage API** - Financial data source

## 📊 Model Architecture

```
Input Layer (20 days of price data)
    ↓
Linear Layer (1 → 32 neurons)
    ↓
ReLU Activation
    ↓
LSTM Layer (32 hidden units, 2 layers)
    ↓
Dropout Layer (20% dropout)
    ↓
Linear Output Layer (32 → 1)
    ↓
Price Prediction
```

## 🔧 Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/ddub227/ibm-lstm-stock-prediction.git
   cd ibm-lstm-stock-prediction
   ```

2. **Install required dependencies**:
   ```bash
   pip install torch numpy matplotlib alpha-vantage
   ```

3. **Get Alpha Vantage API Key** (Optional):
   - Visit [Alpha Vantage](https://www.alphavantage.co/support/#api-key)
   - Get your free API key
   - Replace the demo key in `project.py` (line 19)

## 🚀 Usage

Simply run the main script:

```bash
python project.py
```

The program will:
1. Download IBM stock data from 1999-2025
2. Process and normalize the data
3. Train the LSTM model (100 epochs)
4. Display 4 visualization charts
5. Output the predicted price for the next trading day

## 📈 Model Performance

The model uses the following training configuration:
- **Training/Validation Split**: 80/20
- **Sequence Length**: 20 days
- **Batch Size**: 64
- **Learning Rate**: 0.01 (with step decay)
- **Loss Function**: Mean Squared Error
- **Optimizer**: Adam

## 📊 Output Visualizations

The program generates 4 key visualizations:

1. **Historical Price Chart**: Raw IBM stock prices over 25+ years
2. **Data Split Visualization**: Training vs validation data periods
3. **Model Performance**: Comparison of actual vs predicted prices
4. **Future Prediction**: Next-day price prediction with confidence visualization

## 🎯 Results

The model analyzes patterns in IBM's stock price movements and provides:
- Visual performance metrics on historical data
- Quantitative loss reduction during training
- Next trading day price prediction
- Confidence indicators through visualization

## ⚠️ Important Disclaimers

- **Educational Purpose**: This project is for learning and demonstration only
- **Not Financial Advice**: Predictions should not be used for actual trading decisions
- **Market Risk**: Stock markets are influenced by many factors beyond historical prices
- **No Guarantee**: Past performance does not guarantee future results

## 🔍 Key Learning Concepts

This project demonstrates:
- **Time Series Forecasting** with deep learning
- **LSTM Architecture** for sequential data
- **Data Preprocessing** for financial time series
- **Model Training and Validation** best practices
- **Visualization** of machine learning results

## 📝 Model Limitations

1. **Historical Bias**: Only considers price history, ignores external factors
2. **Lag Effect**: May not capture rapid market movements
3. **Market Complexity**: Real markets influenced by news, sentiment, economics
4. **Overfitting Risk**: Performance on new data may differ from training

## 🔮 Future Enhancements

Potential improvements could include:
- Multiple stock symbols support
- Technical indicators integration
- Sentiment analysis from news/social media
- Fundamental analysis features
- Real-time prediction updates
- Web interface for user interaction

## 📁 Project Structure

```
ibm-lstm-stock-prediction/
│
├── project.py          # Main application file
├── .gitignore         # Git ignore rules
└── README.md          # Project documentation
```

## 📚 Educational Value

This project serves as an excellent introduction to:
- Deep learning with PyTorch
- Financial data analysis
- Time series prediction
- Data visualization
- API integration
- Git/GitHub workflows

## 🤝 Contributing

Feel free to fork this repository and submit pull requests for improvements. Some areas for contribution:
- Code optimization
- Additional visualization features
- Different neural network architectures
- Extended documentation

## 📄 License

This project is open source and available under the MIT License.

## 🙏 Acknowledgments

- Alpha Vantage for providing free financial data API
- PyTorch team for the excellent deep learning framework
- The open source community for inspiration and resources

---

**Built with 🤖 [Claude Code](https://claude.ai/code)**