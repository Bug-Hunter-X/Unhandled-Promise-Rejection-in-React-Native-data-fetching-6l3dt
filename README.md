# Unhandled Promise Rejection in React Native data fetching

This repository demonstrates a common error in React Native applications: attempting to access a property of `null` or `undefined` data before it's been fetched from an API.  The application crashes when the component renders initially and tries to use the data object before the asynchronous `fetch` call completes.

The `bug.js` file contains the buggy code, which fails to properly handle the loading and error states, leading to the crash. The `bugSolution.js` provides a corrected version that addresses these issues using optional chaining and a better error handling mechanism. 