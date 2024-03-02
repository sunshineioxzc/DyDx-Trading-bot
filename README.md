## DyDx Trading bot with custom SDK for API V3

### Overview
This dYdX trading bot is designed for automated trading on the dYdX decentralized exchange. Written in .NET Core 5, it leverages a custom-written SDK for seamless integration with dYdX's Public and Private API v3. Additionally, it utilizes Nethereum, a .NET library for Ethereum interactions, and RESTful API libraries for efficient communication with external services.
The bot employs a sophisticated trading strategy that incorporates the Moving Average Convergence Divergence (MACD) and Relative Strength Index (RSI) indicators. These indicators are utilized to analyze market trends and identify potential entry and exit points for trades.
Traders have the flexibility to select trading pairs and configure stop-loss and take-profit percentages within the bot's settings. This customization allows traders to set predefined levels at which the bot will automatically execute sell orders to limit losses (SL) or secure profits (TP).

### SDK
```
The SDK encapsulates basic dYdX API calls, simplifying interaction with the exchange.
GET /v3/markets
GET /v3/accounts
GET /v3/accounts/{accountId}
GET /v3/orders
POST /v3/orders
GET /v3/orders/{orderId}
DELETE /v3/orders/{orderId}
GET /v3/fills
GET /v3/fills/{fillId}
GET /v3/balances
GET /v3/trades
GET /v3/trades/{tradeId}
GET /v3/margin-accounts
GET /v3/margin-accounts/{accountId}
GET /v3/margin-accounts/{accountId}/positions
GET /v3/margin-accounts/{accountId}/positions/{positionId}
GET /v3/margin-accounts/{accountId}/orders
POST /v3/margin-accounts/{accountId}/orders
GET /v3/margin-accounts/{accountId}/orders/{orderId}
DELETE /v3/margin-accounts/{accountId}/orders/{orderId}
GET /v3/margin-accounts/{accountId}/fills
GET /v3/margin-accounts/{accountId}/fills/{fillId}
GET /v3/markets/{marketId}/orderbook
GET /v3/markets/{marketId}/candles
GET /v3/markets/{marketId}/stats
GET /v3/markets/{marketId}/trades
GET /v3/markets/{marketId}/trades/{tradeId}
GET /v3/protocol/stats
GET /v3/protocol/health
GET /v3/protocol/accounts
```

### Technologies used
- .NET Core 5
- Nethereum
- Newtonsoft.Json
- RestSharp

### Configuration
- RPC (Moralis or private)
- Ethereum private key (Dont use your main wallet)
- Set stop-loss and take-profits precentage


## License

This project is licensed under the (c) 2024 Steve Norman - see the [LICENSE](LICENSE) file for details.
