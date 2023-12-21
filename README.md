# FX Rover P MT4

This code is an example of how the FX Rover P MT4 expert advisor functions. This expert advisor places pending buy and sell orders at specified grid levels within a defined range. 

## Trading Parameters

- LotSize: The initial lot size for the orders
- GridStep: The grid step in pips between each order
- RangeSize: The size of the range in pips

## Trading Function

The `TradeFXRoverP` function is responsible for executing the trading logic. It first calculates the range boundaries based on the current ask and bid prices. 

If the current ask price is higher than the range bottom and the bid price is lower than the range top, it proceeds to calculate the number of grid levels based on the range size and the grid step.

Next, it iterates through each grid level and calculates the buy and sell prices. It then attempts to place a pending buy order and a pending sell order at each grid level. If the order placement is successful, it prints a message indicating the order price.

## Expert Initialization

The `OnInit` function is called during the expert advisor initialization process. It simply prints a message indicating that the expert advisor has been initialized.

## Expert Tick Function

The `OnTick` function is called on each tick of the market data. It calls the `TradeFXRoverP` function to execute the trading logic.

## Expert Deinitialization

The `OnDeinit` function is called during the expert advisor deinitialization process. It prints a message indicating that the expert advisor has been deinitialized.

---

## Product Description

The FX Rover P MT4 is an expert advisor designed to automate trading on the MetaTrader 4 platform. It is developed by the Forex Robot Easy Team.

This expert advisor utilizes a grid trading strategy within a specified range. It places pending buy and sell orders at predefined grid levels. The lot size, grid step, and range size can be customized to suit individual trading preferences.

The FX Rover P MT4 is designed to take advantage of price fluctuations within the defined range, aiming to capture profits as the market moves up and down. It is suitable for both experienced traders looking to automate their trading strategies and beginners seeking a reliable and user-friendly trading solution.

Please note that Forex Robot Easy is not the official developer of this product. We provide this code as an example of how the FX Rover P MT4 expert advisor can function. For detailed reviews and trading results of this product, please visit the official developer's website at [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/review-fx-rover-p-mt4-improved-performance-real-results/). To find the official developer of this product, please use the MQL5 platform.
