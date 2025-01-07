# Expo useAsyncStorage Performance Issue with Large Data

This repository demonstrates a performance problem encountered when using Expo's `useAsyncStorage` hook with substantial data. The issue stems from inefficient state management within the hook, particularly noticeable on lower-end devices.  The app may experience slow loading times, freezes, or unexpected crashes.  Debugging is challenging as no consistent error message is generated.

## Reproduction

1. Clone this repository.
2. Install dependencies using `npm install` or `yarn install`.
3. Run the app using `expo start`.
4. Observe the performance, especially on a lower-end device or when manipulating large datasets. The impact will increase the larger the stored data.

## Solution

The provided solution involves using a more efficient data storage and retrieval method. We'll opt for alternative approaches to mitigate the performance issues, such as data compression, batching, or utilizing a database like SQLite for improved performance with large datasets.