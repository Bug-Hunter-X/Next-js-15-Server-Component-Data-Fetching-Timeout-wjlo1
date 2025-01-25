# Next.js 15 Server Component Data Fetching Timeout

This repository demonstrates an uncommon bug in Next.js 15 related to server components and complex asynchronous data fetching.  When server components perform nested asynchronous operations or recursive calls that trigger additional data fetches, exceeding the default request timeout or encountering unexpected behavior from the data fetching mechanisms becomes possible. 

The `serverComponentBug.js` file contains a simplified reproduction of this issue.  The `serverComponentBugSolution.js` offers a solution using appropriate error handling and request timeouts.