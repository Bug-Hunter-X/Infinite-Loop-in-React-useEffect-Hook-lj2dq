# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by missing dependencies.

## The Bug

The `bug.js` file contains a component that uses the `useEffect` hook to log the current count.  However, it omits the dependency array, resulting in the effect running after every render, and in turn causing a re-render which infinitely repeats.