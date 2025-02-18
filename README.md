# Stocks Analysis AI Agents

This Streamlit app leverages three AI agents to fetch, analyze, and visualize stock market data. It offers an interactive dashboard for quick insights and comprehensive analysis.

## Overview

Users can enter a company name or ticker symbol to receive:
- **Current Stock Price** and key metrics (e.g., forward P/E ratio, recommendations)
- An interactive **candlestick chart** displaying 1-year historical data
- A brief **company overview** if available

The application combines financial data retrieval with web search to deliver a well-rounded analysis.

## AI Agents

- **Web Search Agent:**  
  Uses tools like GoogleSearch and DuckDuckGo to gather additional market context and news.

- **Financial AI Agent:**  
  Utilizes yfinance (via YFinanceTools) to fetch detailed financial metrics and historical stock data.

- **Stock Market Agent:**  
  Integrates the capabilities of both the Web Search and Financial agents to generate a holistic stock analysis.

## Setup & Usage

1. **Installation:**
   ```bash
   pip install streamlit pandas plotly yfinance
2. **Set your api key:**
GROQ_API_KEY = "YOUR_GROQ_API_KEY"

3. **Run the app:**
streamlit run your_app_file.py
##
Enter a stock name or ticker (e.g., APPLE, TCS) and click Analyze to view key metrics, charts, and company details.

**Code Highlights**

**initialize_agents()**:
Sets up the three agents with their respective roles and tools.

**get_stock_data(symbol)**:
Retrieves both current stock info and a year’s worth of historical data using yfinance.

**create_price_chart(hist_data, symbol)**:
Generates a candlestick chart with Plotly for visualizing stock performance.

Contributions and improvements are welcome!
