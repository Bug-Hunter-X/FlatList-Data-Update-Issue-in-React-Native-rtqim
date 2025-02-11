# React Native FlatList Data Update Issue

This repository demonstrates a common issue encountered when using the FlatList component in React Native: failure to properly update the display when the underlying data changes rapidly.

## Problem
The provided `bug.js` file contains a simple example. A `FlatList` is populated with dynamically generated data that updates every second. However, due to FlatList's optimization strategies, the UI often fails to reflect these changes accurately, leading to stale data being displayed.

## Solution
The `bugSolution.js` file presents a solution to address this issue.  The key is to use the `extraData` prop of the FlatList to force a re-render whenever the data changes. 