# Crypto Real-Time Tracker Pro

A comprehensive real-time cryptocurrency tracking application with advanced technical analysis capabilities.

## Features

### 🔴 Real-Time Data
- **WebSocket Integration**: Live price updates from Binance with < 1 second latency
- **Auto-Reconnection**: Exponential backoff reconnection strategy
- **Visual Indicators**: Real-time price change indicators (▲/▼)
- **Update Counter**: Track number of real-time price updates

### 📊 Complete Technical Analysis

#### Fibonacci Analysis
- **Retracement Levels**: 0%, 23.6%, 38.2%, 50%, 61.8%, 78.6%, 100% (ATH to ATL)
- **Extension Levels**: 127.2%, 161.8%, 200%, 261.8% for price targets
- **Visual Indicators**: Color-coded levels with current position highlighting

#### Technical Indicators
- **Moving Averages**: MA 20, 50, 100, 200 with trend comparison
- **RSI (Relative Strength Index)**: 14-period RSI with overbought/oversold indicators
- **MACD**: Moving Average Convergence Divergence with histogram
- **Support & Resistance**: Automatic identification based on Fibonacci levels

### 🎨 Enhanced UI/UX
- **Dark Theme**: Professional dark theme optimized for extended viewing
- **Sortable Columns**: Click any column header to sort data
- **Favorite System**: Star/unstar coins with localStorage persistence
- **Search & Filters**: 
  - Text search for coin symbols
  - Fibonacci distance filters (0-5%, 5-10%, 10-20%, etc.)
  - Favorites-only filter
- **Expandable Details**: Click "View" to see complete technical analysis
- **Responsive Design**: Mobile-friendly layout
- **Color Coding**:
  - Green badges for positive % changes
  - Red badges for negative % changes
  - Real-time price arrows (▲ up, ▼ down)

### 💾 Data Management
- **localStorage**: Persistent favorites across sessions
- **Simulated Historical Data**: For technical indicator calculations
- **Market Cap Display**: Shows market capitalization for each coin
- **ATH/ATL Tracking**: All-time high and low prices from CoinGecko

## Supported Cryptocurrencies

The tracker supports 30+ major cryptocurrencies including:
- Bitcoin (BTC)
- Ethereum (ETH)
- BNB
- Solana (SOL)
- XRP
- Cardano (ADA)
- Dogecoin (DOGE)
- TRON (TRX)
- And many more...

## Files

- **index.html**: Production version with live Binance API and CoinGecko data
- **demo.html**: Demo version with mock data for testing (no API dependencies)

## Usage

### Live Version
Open `index.html` in a web browser. The application will:
1. Fetch ATH/ATL data from CoinGecko API
2. Get current prices from Binance API
3. Establish WebSocket connection for real-time updates
4. Calculate all technical indicators
5. Display sortable, filterable data table

### Demo Version
Open `demo.html` for a fully functional demo with simulated data and live price updates every 3 seconds.

## Features Overview

### Main Dashboard
- Displays all coins with current prices, ATH, ATL, Fibonacci 50%, and market cap
- Real-time WebSocket status indicator
- Live update counter
- Search and filter controls

### Detailed View (Click "View" button)
Each coin's detail panel shows:
1. **Fibonacci Retracement Levels**: All 7 key levels with prices
2. **Fibonacci Extension Levels**: 4 upside targets
3. **Moving Averages Grid**: MA 20, 50, 100, 200
4. **Technical Indicators**: RSI and MACD with visual bars
5. **Coin Information**: Symbol, price, market cap, % from ATH/ATL
6. **Support & Resistance**: Key levels for trading

## Technical Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **APIs**: 
  - Binance API (24hr ticker, WebSocket streams)
  - CoinGecko API (ATH/ATL historical data)
- **Real-time**: WebSocket protocol for live price updates
- **Storage**: localStorage for user preferences
- **Styling**: Custom CSS with gradient themes, responsive design

## Performance

- Real-time updates: < 1 second latency
- WebSocket connection: Auto-reconnect with exponential backoff
- Efficient rendering: Only re-renders filtered/visible data
- Optimized API calls: Rate limiting and caching

## Browser Compatibility

Works in all modern browsers:
- Chrome/Edge (recommended)
- Firefox
- Safari
- Opera

## License

Open source - feel free to use and modify.

## Credits

- Price data: Binance API
- ATH/ATL data: CoinGecko API
- Design: Custom dark theme optimized for crypto trading
