# Node.js 'listen EADDRINUSE' Error
This repository demonstrates a common Node.js error: 'listen EADDRINUSE'. This error occurs when a server attempts to bind to a port that's already in use by another process.  The solution shows how to handle this situation gracefully.

## Bug
The `bug.js` file contains a simple HTTP server that attempts to listen on port 8080. If another application is already using this port, the server will throw the 'listen EADDRINUSE' error.

## Solution
The `bugSolution.js` file demonstrates a more robust approach.  It attempts to bind to the port, and if the error occurs, it waits a short period before retrying.