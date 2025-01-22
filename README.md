# React useEffect Cleanup Function Issue

This repository demonstrates a common issue with the React `useEffect` hook's cleanup function.  The provided code snippet showcases a scenario where the cleanup function isn't consistently executed, leading to potential memory leaks or unintended side effects.

The `bug.js` file contains the problematic code, while `bugSolution.js` provides a corrected version. The issue is related to the timing and conditions under which the cleanup function is triggered.  Understanding how to correctly implement cleanup functions is crucial for writing efficient and reliable React applications.

## Problem
The original code shows a simple counter component. It uses an useEffect hook to log the count to console and include a cleanup function. However, the cleanup function is not being executed every time as expected, causing the console logs to appear in an unpredictable order.  This is a simplified example, but similar issues can appear in more complex scenarios where cleanup isn't properly handled.