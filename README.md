# Missing Dependency in useEffect Hook

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  Forgetting to include state variables in the dependency array leads to unexpected behavior, often an infinite render loop. This example showcases the issue and its resolution. 

## Bug

The `bug.js` file contains a component with a `useEffect` hook that's missing a crucial dependency. This results in the effect running on every render, leading to an infinite loop and console spam.

## Solution

The `bugSolution.js` file provides the corrected code. By including `count` in the dependency array, the effect now only runs when `count` changes, resolving the infinite loop problem. 
