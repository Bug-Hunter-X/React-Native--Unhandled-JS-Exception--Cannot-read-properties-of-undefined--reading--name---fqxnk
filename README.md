# React Native: Handling Null or Undefined Property Access

This repository demonstrates a common React Native error and its solution: attempting to access a property of an object that is `null` or `undefined`.  The error message can be cryptic, making debugging challenging.  The example shows a component that fetches user data asynchronously.  Without proper error handling, trying to access user properties before the data is fetched results in an unhandled JS exception.

The solution employs optional chaining and nullish coalescing to gracefully handle cases where the `user` object or its properties might be undefined.

## Steps to Reproduce

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npx react-native run-android` (or `npx react-native run-ios`).
4. Observe the error initially, then see how the solution resolves it.

## Solution

The solution utilizes optional chaining (`?.`) and the nullish coalescing operator (`??`) to provide robust null and undefined checks before accessing the 'name' property.