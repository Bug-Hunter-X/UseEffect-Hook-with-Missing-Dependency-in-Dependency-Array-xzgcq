# React useEffect Hook with Missing Dependency
This repository demonstrates a common error in React's `useEffect` hook: a missing dependency in the dependency array. This leads to unexpected behavior, often an infinite render loop.

## Bug
The `bug.js` file contains a component that uses `useEffect` to log the current count.  However, the dependency array is missing `count`, causing the effect to run on every render, creating an infinite loop in the console.