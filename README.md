# React useEffect Infinite Loop
This repository demonstrates a common React bug: an infinite loop caused by incorrectly updating state within the useEffect dependency array. The `bug.js` file contains the buggy code, while `bugSolution.js` provides the corrected version.

## Bug Description
The `useEffect` hook is used to update the `count` state variable.  However, the state is updated within the dependency array, resulting in an infinite loop because the `count` variable will continuously change, triggering the useEffect infinitely.