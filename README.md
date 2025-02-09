# React useEffect Runs on Every Render

This repository demonstrates a common issue with the React `useEffect` hook: unintended re-renders even when the dependency array is specified.  The example showcases a counter component where the `useEffect` hook logs the count to the console after every render, which is inefficient and can lead to performance issues in more complex applications.

The solution shows how to correctly use the dependency array to only re-run the effect when the count changes.  This ensures efficiency and avoids unnecessary operations.

## How to reproduce the bug
1. Clone this repository
2. Run `npm install`
3. Run `npm start`
4. Observe the console logs for each click, even on initial render.

## How to fix the bug
Examine the `bugSolution.js` file to see the improved implementation, which only executes the effect when the `count` changes. 