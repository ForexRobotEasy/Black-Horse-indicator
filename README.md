# Black Horse Indicator ReadMe

## Overview
The Black Horse Indicator is a custom-built technical analysis tool developed by the Forex Robot Easy Team. This indicator is designed to identify bullish and bearish divergence patterns in the financial markets, providing traders with potential trading opportunities.

For detailed reviews and trading results of this product, please visit the official website: [Black Horse Indicator Review - Precision Forex Trading Tool](https://forexroboteasy.com/forex-robot-review/black-horse-indicator-review-precision-forex-trading-tool/)

Please note that Forex Robot Easy is not the official developer of this product. We are showcasing a sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

## Code Description
The Black Horse Indicator code is written in MQL4 language. It utilizes the MetaTrader 4 platform's built-in functions and features to calculate and display divergence patterns on the price chart.

### Input Parameters
The indicator has two configurable input parameters:
- LookbackPeriod: Specifies the number of periods to look back for divergence identification. Default value is set to 14.
- ATRMultiplier: Specifies the multiplier used to calculate the threshold for divergence identification. Default value is set to 2.0.

### Indicator Buffers
The indicator utilizes two indicator buffers to store the bullish and bearish divergence pattern values:
- bullishDivergenceBuffer: Stores the values for bullish divergence patterns.
- bearishDivergenceBuffer: Stores the values for bearish divergence patterns.

### Initialization Function (OnInit)
The OnInit function is called during the indicator initialization process. In this function, the indicator buffers are set and labeled for proper display on the price chart.

### Iteration Function (OnCalculate)
The OnCalculate function is called on each new tick or bar. This function calculates the Average True Range (ATR) and uses it to determine divergence patterns. The ATR is calculated using the CopyBuffer function, and divergence patterns are identified based on the price difference and the ATR threshold.

- ATR Calculation: The ATR is calculated using the LookbackPeriod parameter and stored in the atrBuffer array.
- Divergence Calculation: For each bar, the function compares the price difference between the current bar and the LookbackPeriod bars ago with the ATR threshold. If the price difference exceeds the threshold, a bullish or bearish divergence pattern is identified and stored in the respective indicator buffers.

## Usage
To use the Black Horse Indicator, follow these steps:
1. Install the indicator on your MetaTrader 4 platform.
2. Configure the input parameters according to your preferences.
3. Monitor the price chart for bullish and bearish divergence patterns identified by the indicator.
4. Consider these patterns as potential trading opportunities and apply your own trading strategy to make trading decisions.

Please note that the Black Horse Indicator is a tool for technical analysis and should be used in conjunction with other indicators, analysis techniques, and risk management strategies to make informed trading decisions.

## Disclaimer
Forex Robot Easy is not the official developer of the Black Horse Indicator. The provided code is a sample representation of how the indicator may work. For the official version and developer, please refer to the MQL5 platform.

Forex trading involves substantial risk and may not be suitable for all investors. Before engaging in any trading activities, it is important to understand the risks involved and seek professional advice if necessary.
