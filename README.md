# Expo Linking.getInitialURL() Intermittent Null Return

This repository demonstrates a bug in Expo's `Linking.getInitialURL()` API where it inconsistently returns `null`, even when a deep link is successfully opened. This makes handling deep links unreliable.

## Reproducing the Bug

1. Clone this repository.
2. Run the app in an Expo Go client or on a device.
3. Open a deep link targeting the app (e.g., `exp://your-app-id`).
4. Observe the console output.  The `getInitialURL()` call may or may not return the deep link URL.

## Workaround (see bugSolution.js)