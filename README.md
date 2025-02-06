# React useEffect Conditional Rendering Bug

This repository demonstrates a common bug in React applications involving incorrect conditional rendering logic within the `useEffect` hook.  The bug can lead to unexpected behavior or, in some cases, infinite loops. The solution provides a corrected implementation.

## Bug

The initial implementation includes a conditional statement within the `useEffect` hook that only logs a message to the console if the `count` state variable is greater than 0. This approach is flawed because the effect runs every time the `count` changes, potentially leading to unintended side effects.

## Solution

The solution refactors the conditional rendering logic to avoid unnecessary re-renders and potential infinite loops. The effect is optimized to run only when necessary, improving performance and avoiding unexpected behavior.