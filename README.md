# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving an infinite loop caused by the incorrect use of the `useEffect` hook's dependency array. The `bug.js` file contains the buggy code, while `bugSolution.js` provides the corrected version.

## Bug Description

The `useEffect` hook in `bug.js` attempts to log the `count` value whenever it changes.  However, the dependency array `[count]` causes the effect to run every time `count` updates, triggering a re-render, leading to an infinite loop.

## Solution

The `bugSolution.js` file fixes this by optimizing the use of `useEffect`.  The dependency array can be omitted to run only after each render or specific other dependencies can be added.
