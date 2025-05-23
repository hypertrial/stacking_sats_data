# Stacking Sats Data Engineering

This repository contains data engineering tools and pipelines for the [Hypertrial Stacking Sats Challenge](https://github.com/hypertrial/stacking_sats_challenge).

## Overview

The Stacking Sats Challenge focuses on developing dynamic Bitcoin accumulation strategies that outperform standard Dollar Cost Averaging (DCA). This repository provides the data infrastructure needed to develop, test, and optimize these strategies.

## Data Sources

- **Bitcoin Price Data**: Historical BTC price data from CoinMetrics
- **Market Indicators**: Various technical and fundamental indicators for strategy development
- **On-chain Metrics**: Bitcoin network data for advanced strategy development

## Tools

### CoinMetrics Data Extractor

`coinmetrics.py` is a robust tool for downloading and processing Bitcoin data from CoinMetrics:

```bash
# Basic usage
python coinmetrics.py

# Custom output paths
python coinmetrics.py --csv custom_btc.csv --parquet custom_btc.parquet

# Skip CSV output
python coinmetrics.py --csv none
```

### Features

- Robust error handling for network and parsing issues
- Support for both CSV and Parquet formats
- Configurable data sources and outputs
- Detailed logging

## Getting Started

1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run the data extraction tools to build your dataset
4. Use the prepared data for your strategy development

## Integration with Challenge

This data engineering toolkit is designed to support the [Hypertrial Stacking Sats Challenge](https://github.com/hypertrial/stacking_sats_challenge), providing clean, reliable data for strategy development and backtesting.

## License

MIT License
