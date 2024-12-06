# AsyncStorage getItem Returns Null in Expo

This repository demonstrates a problem and its solution related to AsyncStorage in Expo. The issue involves AsyncStorage.getItem consistently returning null, even after successfully using AsyncStorage.setItem.

## Problem
The core problem is that AsyncStorage.getItem seems to be unable to retrieve data that is successfully stored using AsyncStorage.setItem.  Console logs confirm that setItem works as expected, but getItem persistently returns null.

## Solution
The solution involves ensuring that the keys used for both setItem and getItem are identical, and carefully handling potential asynchronous operations. The example shows the proper usage and error handling for AsyncStorage.