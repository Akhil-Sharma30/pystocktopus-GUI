# PYSTOCKTOPUS GUI Application

This repository contains a Python GUI application that provides a user-friendly interface to interact with the `pystocktopus` package. The GUI enables users to easily generate stock CSV files, predict next-day closing prices, and perform news analysis for stocks by interacting with APIs like Polygon.io and NewsAPI.

The application is built using the `tkinter` library for the GUI and integrates with the `pystocktopus` package for backend stock data extraction, prediction, and analysis.

## Features

- **API Key Submission**: Submit your API keys for Polygon.io and NewsAPI directly through the GUI.
- **Stock CSV Generator**: Generate a CSV file containing stock data for a given date range, ticker, timespan, and multiplier.
- **Next-Day Stock Prediction**: Predict the next day's stock closing price using an LSTM model, trained with custom parameters such as epochs and learning rate.
- **News Analysis**: Analyze recent news for a specific stock, with an option to select the timeframe and extract sentiment analysis.

## Prerequisites

To run this application, you need the following:

- **Python 3.7+**
- **API keys for [Polygon.io](https://polygon.io/) and [NewsAPI](https://newsapi.org/)**

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/pystocktopus-gui.git
   cd pystocktopus-gui
   ```

2. Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Install `pystocktopus` via `pip`:

   ```bash
   pip install pystocktopus
   ```

4. You will also need the `tkinter` and `tkcalendar` modules:

   ```bash
   pip install tk tkcalendar
   ```

## Usage

1. Run the Python script:

   ```bash
   python main.py
   ```

2. Upon first launch, you will be prompted to enter your **Polygon.io** and **NewsAPI** API keys. These keys will be saved in a `.env` file for future use.

3. After successful API key submission, you will be taken to the main menu, where you can:

   - **Generate CSV for Stock Data**: Input stock ticker, timespan, and date range, and generate a CSV file with stock data.
   - **Predict Next-Day Closing Price**: Upload a CSV file, specify the model parameters (epochs, learning rate, etc.), and get the predicted closing price.
   - **Analyze Stock News**: Input stock name and timeframe to analyze recent news for sentiment.

## Files

- **`main.py`**: Main Python script containing the GUI implementation.
- **`.env`**: Environment file for storing API keys (automatically generated after first launch).

## Requirements

- **pystocktopus** (Core library for stock data extraction, news analysis, and stock forecasting)
- **tkinter** (Python's standard GUI library)
- **tkcalendar** (For calendar widgets in the GUI)
- **dotenv** (To manage environment variables)

## Acknowledgments

This application is built on top of the [`pystocktopus`](https://pypi.org/project/pystocktopus/) library. Special thanks to the developers for providing a powerful API to work with stock data, news analysis, and predictions.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.