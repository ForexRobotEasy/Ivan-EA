# Ivan EA ReadMe File

This ReadMe file provides an overview of the Ivan EA code and describes how it works. Please note that ForexRobotEasy is not the official developer of this product. We are only providing a sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

## Code Overview

The Ivan EA is an Expert Advisor (EA) for the MetaTrader 5 platform. It utilizes the RSI (Relative Strength Index) and EMA (Exponential Moving Average) indicators to determine market trends and open positions accordingly. The code is structured with necessary libraries, constants, and event handlers.

### Libraries Used:

- `PositionInfo.mqh`: Provides functions related to position information.
- `OrderInfo.mqh`: Provides functions related to order information.

### Constants Defined:

- `RSI_PERIOD`: Defines the period for calculating the RSI indicator.
- `EMA_PERIOD`: Defines the period for calculating the EMA indicator.
- `PULLBACK_LIMIT`: Defines the maximum allowed pullback percentage from the EMA.
- `STOP_LOSS`: Defines the number of pips for the stop loss level.
- `TAKE_PROFIT`: Defines the number of pips for the take profit level.

### OnTick Event:

The `OnTick()` function is the main event handler, which is called on every tick of the price data. In this event, the code performs the following steps:

1. Get the current RSI and EMA values.
2. Get the current bar price.
3. Determine the market trend based on RSI and EMA values.
4. Check if the current price is within the allowed pullback limit from the EMA.
5. If there are no open positions and the conditions for opening a new position are met, the code opens a new position with the specified parameters.
6. If there are open positions, the code checks for exit conditions and closes the positions if the stop loss or take profit levels are reached.

### OnDeinit Event:

The `OnDeinit()` function is called when the EA is being unloaded or deactivated. It can be used for cleanup code if required.

### OnInit Event:

The `OnInit()` function is called when the EA is initialized. It can be used for initialization code if required.

## Product Description

The Ivan EA is a smart Forex trading robot that utilizes custom tools to make trading decisions. It combines the RSI and EMA indicators to identify market trends and open positions accordingly. This EA is designed to work on the MetaTrader 5 platform and can be used for automated trading in the Forex market.

Key Features:
- Utilizes the RSI and EMA indicators for accurate market analysis.
- Opens positions based on predefined conditions and pullback limits.
- Implements stop loss and take profit levels for risk management.
- Provides detailed logs of position openings and closings.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Ivan EA Review](https://forexroboteasy.com/forex-robot-review/ivan-ea-review-smart-forex-trading-with-custom-tools/). Please note that ForexRobotEasy is not the official developer of this product. We are only showcasing a sample code that demonstrates how this product can work. To find the official developer of this product, please use MQL5.
