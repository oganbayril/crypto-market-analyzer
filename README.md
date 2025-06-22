# Crypto Market Analyzer 📈

A comprehensive cryptocurrency analysis tool that fetches real-time data from the CoinGecko API to analyze market trends, price movements, and generate insightful visualizations for the top cryptocurrencies by market cap.

## Features

🔍 **Market Cap Analysis**
- Display top N cryptocurrencies by market capitalization
- Show current prices and market cap values
- Real-time data fetching from CoinGecko API

📊 **Daily Price Tracking**
- Generate detailed graphs showing 30-day price movements
- Display both absolute price changes and percentage changes day-by-day
- Interactive visualizations for better data interpretation

📈 **Performance Overview**
- Create summary graphs showing total 30-day percentage change
- Compare starting prices (30 days ago) with current prices
- Clear visualization of overall performance trends

## Prerequisites

Before running this project, make sure you have the following installed:

- Python 3.7+
- Jupyter Notebook or JupyterLab
- Required Python packages (see Installation section)

## Installation

1. Clone this repository:
```bash
git clone https://github.com/oganbayril/crypto-market-analyzer.git
cd crypto-market-analyzer
```

2. Install required packages::
```bash
pip install -r requirements.txt
```

## Usage

### Running the Analysis

1. Launch Jupyter Notebook:
```bash
jupyter notebook
```

2. Open the `crypto_market_analyzer.ipynb` file

3. Execute all cells in order by clicking "Run All" or run cells individually

### Customization

You can customize the analysis by modifying these parameters in the notebook:

- **Number of coins**: Change the `top_n_coins_input` parameter to analyze more or fewer cryptocurrencies
- **Time period**: Modify the date range for historical data analysis
- **Visualization style**: Adjust graph colors, sizes, and styling options

## API Information

This project uses the **CoinGecko Public API** which provides:
- Real-time cryptocurrency data
- Historical price information
- Market capitalization data
- No API key required for basic usage

**API Rate Limits**: CoinGecko's public API has rate limits. The code includes appropriate delays to respect these limits.

## Output Examples

The analyzer generates three main types of output:

1. **Market Cap Table**: A formatted display of top cryptocurrencies with their market cap and current prices

2. **Daily Price Charts**: Individual graphs for each cryptocurrency showing:
   - 30-day price movement timeline
   - Daily percentage changes
   - Price trend visualization

3. **Performance Summary**: Overview charts displaying:
   - Total 30-day percentage change
   - Starting vs. current price comparison
   - Performance ranking among analyzed coins

## Project Structure

```
crypto-market-analyzer
│
├── crypto-market-analyzer.ipynb    # Main analysis notebook
├── README.md                       # Project documentation
└── requirements.txt               # Python dependencies
```

## Technical Details

- **Data Source**: CoinGecko Public API
- **File Format**: Jupyter Notebook (.ipynb)
- **Primary Libraries**: 
  - `requests` for API calls
  - `pandas` for data manipulation
  - `matplotlib`/`seaborn` for visualizations
  - `numpy` for numerical operations

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [CoinGecko](https://www.coingecko.com/) for providing free cryptocurrency API
- The Python data science community for excellent visualization libraries

## Disclaimer

This tool is for educational and informational purposes only. It should not be used as the sole basis for investment decisions. Cryptocurrency investments carry significant risks, and past performance does not guarantee future results.

---

**Note**: Make sure to run all cells in the notebook sequentially for proper execution. The analysis is dynamic and will fetch the most current data available from the CoinGecko API.
