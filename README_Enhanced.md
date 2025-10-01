# Enhanced Jesse Trading Bot

## Overview

This is an enhanced version of the Jesse trading framework with multi-asset support including cryptocurrencies, stocks, options, and futures. The system includes:

- **Multi-Source Data Feeds**: Kraken, Binance, Tradier, DexScreener, CoinGecko
- **Paper Trading Engine**: Risk-free strategy testing with realistic simulation
- **Live Trading Support**: Real money trading with comprehensive risk management
- **Backtesting System**: Historical strategy validation and optimization
- **Multi-Asset Support**: Crypto, stocks, options, futures, and launchpad tokens

## Key Features

### Data Sources
- **Kraken**: Major crypto exchange WebSocket feeds (FREE)
- **Binance**: World's largest crypto exchange (FREE)
- **Tradier**: US stocks, options, futures (FREE sandbox)
- **DexScreener**: Launchpad token data (FREE)
- **CoinGecko**: Additional crypto market data (FREE)

### Trading Modes
- **Paper Trading**: $100K virtual balance for strategy testing
- **Live Trading**: Real money trading with risk controls
- **Backtesting**: Historical data analysis and optimization

### Supported Assets
- **Cryptocurrencies**: BTC, ETH, ADA, SOL, LINK, and 1000+ pairs
- **US Stocks**: SPY, QQQ, AAPL, GOOGL, MSFT, TSLA, etc.
- **Futures**: ES (Mini S&P), MES (Micro S&P), NQ, MNQ, YM, MYM
- **Options**: All US equity options
- **Launchpad Tokens**: New token launches on DEX platforms

## Quick Start

### Installation
```bash
pip install websockets aiohttp matplotlib pandas openpyxl
```

### Configuration
1. Copy `enhanced_data_config.json.example` to `enhanced_data_config.json`
2. Enable desired data sources
3. Add API keys for Tradier (optional)

### Running the System
```bash
# Start data server
python enhanced_data_server.py

# Start paper trading (separate terminal)
python paper_trading_engine.py

# Launch dashboard (separate terminal)
python live_dashboard.py
```

## File Structure

```
enhanced_data_server.py      # Multi-source market data server
enhanced_data_config.json    # Configuration file
paper_trading_engine.py      # Paper trading simulation
live_dashboard.py           # GUI trading dashboard
market_data_client.py       # Client connection examples
STONE_Setup_Manual.md       # Comprehensive setup guide
```

## Performance Tracking

All trading data is automatically exported to Excel with:
- Performance metrics and returns
- Complete order and trade history
- Position tracking and P&L analysis
- Portfolio timeline and risk metrics

## Risk Management

Built-in risk controls include:
- Position size limits (default 5% max per position)
- Portfolio risk limits (default 2% max portfolio risk)
- Automatic stop losses and take profits
- Maximum position and daily trade limits

## Documentation

See `STONE_Setup_Manual.md` for comprehensive setup and usage instructions.

## Support

- Tradier API: https://developer.tradier.com
- Free sandbox accounts available for testing
- All data sources have free tiers for development

## License

This enhanced version maintains compatibility with the original Jesse framework while adding extensive multi-asset capabilities.

## Security Note

This version includes security auditing and malicious code removal for safe operation with real trading accounts.