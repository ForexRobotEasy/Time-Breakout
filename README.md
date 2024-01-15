# Time Breakout ReadMe

This code is an example of a trading strategy called Time Breakout, developed by the Forex Robot Easy Team. It is designed to analyze market volatility during a specific time period and execute trades based on breakout levels.

## Input Parameters

- `StartHour` (default: 8): The start hour for breakout analysis.
- `EndHour` (default: 16): The end hour for breakout analysis.
- `StopLoss` (default: 50): The stop loss in points.
- `TakeProfit` (default: 100): The take profit in points.

## Global Variables

- `tradeTime`: The trade execution time.
- `breakoutLevel`: The optimal breakout level calculated based on the previous candle's price range.

## Initialization Function

The `OnInit` function is called during the expert initialization. It sets the trading time to the current time and calculates the breakout level based on the previous candle's price range. The breakout level is then printed.

## Tick Function

The `OnTick` function is called on each tick of the market. It checks if it's a valid trading time based on the `StartHour` and `EndHour` parameters. If it is, it checks for a breakout opportunity. If the bid price exceeds the breakout level, a buy trade is opened with the specified stop loss and take profit. If the ask price falls below the breakout level, a sell trade is opened with the specified stop loss and take profit.

## Product Description

The Time Breakout strategy is a Forex trading software that aims to take advantage of market volatility during specific time periods. It is designed to identify breakout levels and execute trades accordingly.

This code serves as a sample implementation of the Time Breakout strategy and is not the official product developed by Forex Robot Easy. It is provided as an example to showcase how the strategy can be implemented.

For detailed reviews and trading results of the official Time Breakout Forex software, please visit the [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/time-breakout-forex-software-review-trade-us-market-volatility/) website. To find the official developer of this product, please refer to MQL5.
