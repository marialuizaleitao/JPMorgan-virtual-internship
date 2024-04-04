# Task 3: Display data visually for traders

## Background Information

In the trading analysis and stock price monitoring domain, accessing and adjusting data feeds is vital. With previous tasks completed, the adjusted data set is now piped into Perspective on your system.

Traders require comprehensive views of trading strategies, often displayed across multiple screens with live and historical data. Visualizing data clearly, with considerations for user interface and experience, is crucial for providing traders with tools to enhance their performance.

## Objectives

In this task, we aim to:

1. Enhance the graph's utility for traders by tracking the ratio between two stocks over time, rather than the top_ask_price of each stock.
2. Implement the graph to display upper and lower bounds, indicating historical correlation, and trigger alerts when these bounds are crossed.

## Initial Client State

The initial state of the client resembles the outcome of task 2, displaying two stocks and their top_ask_price changes over time.

## Changes Made

### 1. Graph.tsx
- Modified `componentDidMount` method to update the schema object, configuring the Perspective table view for the graph.
- Adjusted attributes such as `view`, `column-pivots`, `row-pivots`, `columns`, and `aggregates` to reflect the new objectives.
- Updated `componentDidUpdate` method to handle new data.

### 2. DataManipulator.ts
- Updated the `Row` interface to match the new schema.
- Modified the `generateRow` function to process raw server data, computing ratios, upper and lower bounds, and trigger alerts.

## End Result

The graph now accurately tracks the ratio between two stocks over time, displaying upper and lower bounds for historical correlation. Trigger alerts notify traders of potential trading opportunities when these bounds are crossed.

Feel free to experiment with different threshold values to fine-tune alerting behavior.
