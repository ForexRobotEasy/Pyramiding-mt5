# Pyramiding mt5

Pyramiding mt5 is an expert advisor developed by Forex Robot Easy Team. It is designed to boost lot size with trend direction in MetaTrader 5 platform. This code serves as a sample implementation of the expert advisor's functionalities.

## Input parameters
- `enableSeriesInitiation`: Enable or disable series initiation.
- `takeProfit`: Aggregate take profit in deposit currency.
- `lotSizeIncrement`: Lot size increment.
- `maxLotSize`: Maximum lot size.

## Expert initialization function
The `OnInit()` function is called when the expert advisor is initialized. It checks if the account is a hedge type account and performs necessary initialization code.

## Expert deinitialization function
The `OnDeinit()` function is called when the expert advisor is deinitialized. It can be used to perform any necessary deinitialization code.

## Expert start function
The `OnTick()` function is called on each tick and handles trades and series initiation. It checks if all orders are closed and series initiation is enabled, and if so, it calls the `InitiateNewSeries()` function. It also checks if the take profit is reached and closes all orders if necessary.

## Helper functions
- `IsAllOrdersClosed()`: Checks if all orders are closed. Returns `true` if all orders are closed, and `false` otherwise.
- `InitiateNewSeries()`: Initiates a new series of orders. This function can be customized to implement the specific logic for initiating a new series.
- `IsTakeProfitReached()`: Checks if the take profit is reached. Returns `true` if the take profit is reached, and `false` otherwise. This function can be customized to implement the specific logic for checking the take profit.
- `CloseAllOrders()`: Closes all open orders. This function can be customized to implement the specific logic for closing orders.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Pyramiding mt5 Review](https://forexroboteasy.com/forex-robot-review/pyramiding-mt5-review-boosting-lot-size-with-trend-direction/). Please note that ForexRobotEasy is not the official developer of this product. This code is only a sample implementation that demonstrates the functionalities described in the product. To find the official developer of this product, please refer to MQL5.
