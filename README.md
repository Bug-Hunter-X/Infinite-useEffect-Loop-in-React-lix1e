# Infinite useEffect Loop in React

This repository demonstrates a common bug in React applications: an infinite loop caused by an incorrectly used `useEffect` hook.

The `bug.js` file contains the buggy code, where the `useEffect` hook unintentionally triggers an infinite loop due to state update inside the effect's logic.  The `bugSolution.js` file shows the corrected code.

## How to reproduce

1. Clone this repository.
2. Navigate to the directory.
3. Open `bug.js` to observe the buggy code.
4. Run a React development server and see the console log for the effect of the bug.
5. Open `bugSolution.js` to see the correction.

## How to fix

The primary cause of this issue is updating state values within the `useEffect` hook without properly managing dependencies. The solution involves carefully examining the effect's logic and dependencies to avoid triggering unnecessary re-renders and state updates, leading to infinite loops. The corrected code in `bugSolution.js` provides a clear solution and explanation.