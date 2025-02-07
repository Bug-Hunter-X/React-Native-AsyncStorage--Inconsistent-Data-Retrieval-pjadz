# React Native AsyncStorage: Inconsistent Data Retrieval

This repository demonstrates a common, yet subtle bug in React Native's AsyncStorage.  The issue revolves around retrieving data from AsyncStorage;  while the data appears to be stored correctly, retrieval might yield unexpected `undefined` values or incorrect data.  The problem is intermittent and difficult to debug.

## The Bug
The provided `bug.js` file contains code that attempts to store and retrieve a value using AsyncStorage.  Despite apparent successful storage, the retrieved value is sometimes incorrect or `undefined`, even when the storage operation seems successful. This inconsistency makes debugging challenging.

## The Solution
The solution, presented in `bugSolution.js`, addresses this by implementing proper error handling and type checking when retrieving data from AsyncStorage. It emphasizes converting the retrieved string value to the appropriate data type before usage.  This resolves the inconsistent data retrieval problem.

## How to Reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run the React Native project (instructions may vary depending on your project setup).
4. Observe the console logs for inconsistencies in data retrieval.

## Contributing
Contributions are welcome!  If you have any improvements or encounter similar issues, please submit a pull request.