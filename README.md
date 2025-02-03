# Unnecessary Re-renders in React useEffect

This repository demonstrates a common React bug where the `useEffect` hook causes unnecessary re-renders and console logs due to an improperly configured dependency array. The `bug.js` file shows the problematic code, while `bugSolution.js` provides the corrected version.

## Bug Description

The `useEffect` hook in `bug.js` lacks a dependency array, causing it to run after every render. This leads to performance issues and unnecessary console output.

## Solution

The `bugSolution.js` file corrects this by adding `count` to the dependency array. This ensures that the effect only runs when the `count` value changes.