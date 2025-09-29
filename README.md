# 📈 SOX vs DJIA Positive/Negative Return Comparison
# （AI-Powered Analysis of Semiconductor and Index Returns）
### Since the emergence of ChatGPT （2022，11，30） , how have AI-driven SOX and traditional industries performed in terms of returns?  This project is a Streamlit web application for visualizing and comparing the performance of AI-representing SOX and traditional industry DJIA, showing their cumulative returns over different time windows since the advent of ChatGPT.

---

## ✨ Features

* 📊 **Data Fetching**: Automatically download historical data for SOX and DJIA using [yfinance](https://pypi.org/project/yfinance/)
* 🔄 **Time Window Selection**: Choose among

  * Last 1 Month
  * Last 3 Months
  * Last 6 Months
  * Year-to-Date (YTD)
  * Last 1 Year
  * Last 3 Years
* 📈 **Normalized Comparison**: Normalize both indices to 100 at the start for intuitive visual comparison
* ➖ **Difference Analysis**: Compute the difference between SOX and DJIA and show the latest difference value
* 📉 **Cumulative Difference Plot**: Display the cumulative difference over the selected period

## 🌐 Live Demo

Try the app online: [SOX vs DJIA Comparison](https://soxdjia-lax6snjubmposywh7jrfty.streamlit.app/)


---

## 📦 Installation

Make sure you have **Python 3.9+** installed. Then install the required packages:

```bash
pip install -r requirements.txt
```

`requirements.txt` example:

```
streamlit
yfinance
pandas
matplotlib
```

---

## 🚀 Run the App

Run the app in the project directory:

```bash
streamlit run sox_djia.py
```

A browser window will automatically open at [http://localhost:8501](http://localhost:8501).

---

## 📷 Screenshots

### 1. Time Window Selection

Select different time windows on the sidebar:

![time window](docs/screenshot_radio.png)

### 2. Normalized Cumulative Returns

Blue = SOX, Orange = DJIA, Green dashed = Difference:

![comparison](docs/screenshot_comparison.png)

### 3. Cumulative Difference

Green shaded area = cumulative difference of SOX relative to DJIA:

![cumulative diff](docs/screenshot_cumulative.png)

---

## 📁 Project Structure

```
.
├── sox_djia.py         # Main application script
├── README.md           # Project documentation
├── requirements.txt    # Dependencies list
└── docs/               # Optional screenshots folder
```

---

## 🔮 Future Improvements

* [ ] Highlight peak/trough points in AI vs traditional industry performance
* [ ] Add more AI-representative and traditional market indices for comparison (e.g., NASDAQ, S&P 500)
* [ ] Implement backtesting to evaluate hypothetical AI-focused investment strategies

---

## 📝 License

* This project is for educational and research purposes only. Data is sourced from Yahoo Finance.
* Author: Shaoxian Duan
