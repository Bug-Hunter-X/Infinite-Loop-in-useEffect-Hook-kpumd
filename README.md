# React useEffect Infinite Loop Bug
This repository demonstrates a common error in React applications: an infinite loop caused by incorrectly using the `useEffect` hook.

The bug is in `bug.js`. The `useEffect` hook attempts to update the `count` state within its callback, causing an infinite loop because it lacks dependencies, leading to continuous state updates. 

The solution is provided in `bugSolution.js`, showcasing the correct usage of the dependency array to prevent the infinite loop.