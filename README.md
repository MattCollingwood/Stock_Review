# Stock_Review
This is a Stock Tracker desktop application built with the Flet framework that fetches and visualizes real-time stock market data using the Alpha Vantage API.


# 📈 Stock Tracker - Real-Time Stock Data Visualizer

A beautiful, interactive desktop application built with Python and Flet that fetches and visualizes real-time stock market data using the Alpha Vantage API.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Flet](https://img.shields.io/badge/Flet-Latest-purple.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## ✨ Features

- 🔍 **Real-Time Stock Data** - Fetch live stock information for any publicly traded company
- 📊 **Interactive Charts** - Visualize closing prices with beautiful line charts
- ⏱️ **Multiple Time Ranges** - View data from 1 week to 5 years
- 💰 **Price Dashboard** - Display Open, High, Low, and Close prices in an intuitive layout
- 🎨 **Modern UI** - Clean, responsive interface with color-coded price indicators
- ⚡ **Fast & Lightweight** - Built with Flet for smooth desktop performance

## 🖼️ Screenshots

*Add screenshots of your application here*

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- Alpha Vantage API key (free)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/stock-tracker.git
   cd stock-tracker
   ```

2. **Install required packages**
   ```bash
   pip install flet requests
   ```

3. **Get your Alpha Vantage API key**
   - Visit [Alpha Vantage](https://www.alphavantage.co/support/#api-key)
   - Sign up for a free API key
   - Note: Free tier allows 25 requests per day

4. **Configure API key**
   
   Create a `config.py` file in the project root:
   ```python
   API_KEY = "your_api_key_here"
   ```

### Usage

Run the application:
```bash
python main.py
```

**How to use:**
1. Enter a stock symbol (e.g., AAPL, GOOGL, MSFT, TSLA)
2. Select your desired time range from the dropdown
3. Click "Get Stock Data" or press Enter
4. View the interactive chart and price information

## 📋 Supported Time Ranges

- 1 week (7 days)
- 2 weeks (14 days)
- 30 days
- 90 days
- 1 year (365 days)
- 5 years (1825 days)

## 🛠️ Built With

- **[Flet](https://flet.dev/)** - Framework for building interactive multi-platform applications
- **[Alpha Vantage API](https://www.alphavantage.co/)** - Stock market data provider
- **[Requests](https://requests.readthedocs.io/)** - HTTP library for API calls

## 📁 Project Structure

```
stock-tracker/
├── main.py           # Main application file
├── config.py         # API key configuration
├── README.md         # Project documentation
└── requirements.txt  # Python dependencies (optional)
```

## 🔧 Configuration

### Window Settings
You can customize the application window in `main.py`:
```python
page.window_width = 1000   # Adjust width
page.window_height = 1000  # Adjust height
page.theme_mode = ft.ThemeMode.LIGHT  # Change to DARK for dark mode
```

### Chart Styling
Modify chart colors and styling in the `fetch_stock_data` function:
```python
color=ft.Colors.ORANGE,              # Line color
below_line_bgcolor=ft.Colors.ORANGE_100  # Fill color
```

## 🐛 Troubleshooting

**Error: "Invalid API call"**
- Check that your API key is correctly set in `config.py`
- Verify you haven't exceeded the API rate limit (25 calls/day for free tier)

**Error: "Please enter stock symbol"**
- Make sure you've entered a valid stock ticker symbol

**No data displayed**
- Verify the stock symbol exists and is traded on major exchanges
- Check your internet connection

## 📝 API Limitations

- **Free Tier**: 25 API requests per day
- **Rate Limit**: 5 API requests per minute
- Consider upgrading to a premium plan for higher limits


## 📜 License

This project is licensed under the MIT License 

## 🙏 Acknowledgments

- Alpha Vantage for providing the stock market API
- Flet team for the amazing framework
- Python community for excellent libraries
