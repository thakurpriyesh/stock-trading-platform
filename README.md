# 📈 StockPulse 🚀

A simple, single-file full-stack Python 🐍 application that fetches and displays stock data! 💸

This app provides a sleek web interface to view a stock's current price, daily change, and a historical chart with a 20-day moving average. 📊

It uses a Python **Flask** backend to serve the page and securely fetch data from the **Alpha Vantage** API.

## ✨ Features

* **Current Quote:** 💰 View the latest price, daily change, and percent change for any stock ticker.
* **Historical Chart:** 📉 Displays a clean line chart of the last 100 days of closing prices.
* **Trend Analysis:** 🔮 Automatically calculates and overlays a 20-day Simple Moving Average (SMA) so you can spot trends!
* **Dynamic UI:** 💻 The frontend is built with **Tailwind CSS** and **Chart.js** for a modern, responsive, and interactive experience.
* **All-in-One:** 📦 The entire application (backend, frontend, and API logic) is contained in `main.py`.

## 🛠️ Technology Stack

* **Backend:** Python 🐍
    * **Flask:** Lightweight micro-framework for the web server and API routes.
    * **Requests:** Used to make HTTP requests to the external Alpha Vantage API.
* **Frontend:**
    * **HTML5**
    * **JavaScript (ES6+):** 🍦 Handles all the frontend logic, API calls, and chart rendering.
    * **Tailwind CSS:** 🎨 For all the awesome styling and layout.
    * **Chart.js:** 💹 For rendering the beautiful, interactive stock chart.
* **Data Source:**
    * **Alpha Vantage API:** Provides all the stock quote and time series data.

## 🚀 How to Run

1.  **Prerequisites:** You must have **Python 3** installed on your system.
2.  **Install Libraries:** Install the required Python libraries (Flask and Requests).
    ```bash
    pip install Flask requests
    ```
3.  **Run the Server:** Run the `main.py` file from your terminal.
    ```bash
    python main.py
    ```
4.  **View the App:** 🎉 Open your web browser and go to:
    ```
    http://localhost:5000
    ```

## 🔧 Configuration

The Alpha Vantage API key is hardcoded in the `main.py` file:

```python
# Your secret API key is stored securely on the server
ALPHA_VANTAGE_API_KEY = "AF01F23GQ79IIP3X"
```

If the application stops working or you hit a rate limit, you may need to get your own free API key from Alpha Vantage and replace the one in the file.

