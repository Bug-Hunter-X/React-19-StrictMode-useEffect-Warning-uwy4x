# React 19 StrictMode useEffect Warning

This repository demonstrates a common issue encountered when using `useEffect` hooks within React 19's StrictMode.  StrictMode adds additional checks that can highlight potential performance problems or unexpected behavior.

The `bug.js` file shows code that triggers a warning in StrictMode due to unnecessary renders within `useEffect`. The solution demonstrates how to prevent such warnings and improve performance.

## How to reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console warnings when using StrictMode.
5. Compare the behavior of the `bug.js` and `bugSolution.js` components.

## Solution

The solution involves using the `count` variable in the dependency array of `useEffect` to ensure the effect runs only when the `count` variable changes. This prevents unnecessary calls and improves the performance of the component. 