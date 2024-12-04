# Node.js Server Not Listening on Specified Port

This repository demonstrates a common issue in Node.js where a server fails to listen on the specified port after calling `server.listen()`.  This can happen for several reasons, primarily because the port is already in use by another process or due to insufficient operating system privileges. The solution involves checking for port availability and handling errors gracefully.

## Bug

The `server.js` file contains a simple HTTP server.  However, if the port 8080 is already in use, the server will fail to start without explicitly handling the error.

## Solution

The `serverSolution.js` file demonstrates a more robust approach. It includes error handling to detect if the port is in use and provides a more informative message to the user.