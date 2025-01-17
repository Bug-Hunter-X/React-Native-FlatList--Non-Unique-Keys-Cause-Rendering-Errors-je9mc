# React Native FlatList: Non-Unique Keys Cause Rendering Errors

This repository demonstrates a common error in React Native's FlatList component: using non-unique keys for items.  This can lead to unexpected behavior, including incorrect rendering and performance issues. 

## Bug Description
Using the index as a key in FlatList, while seemingly convenient, is problematic when items are added or removed from the data array. This leads to incorrect updates and rendering glitches.

## Solution
Use unique identifiers for each item.  Ideally, this would be a unique ID from your data source (e.g., database ID).

## How to Reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run the app on an emulator or device.
4. Observe the erratic behavior of the FlatList when items are added or removed from the data.