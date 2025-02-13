# Node.js Server Port Already in Use Error

This repository demonstrates a common error in Node.js: attempting to start a server on a port that is already in use.  The `bug.js` file contains the problematic code, while `bugSolution.js` offers a solution.

## Bug

The `bug.js` file creates an HTTP server and attempts to listen on port 8080. If another application is already using this port, the server will fail to start and an error will be thrown.  This error is often difficult to debug for beginners.

## Solution

The `bugSolution.js` demonstrates a robust solution. It handles the `EADDRINUSE` error gracefully, retrying the server startup after a short delay. This prevents the application from crashing and allows for a more user-friendly experience.