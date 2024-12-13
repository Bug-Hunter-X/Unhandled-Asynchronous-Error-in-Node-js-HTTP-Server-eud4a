# Unhandled Asynchronous Error in Node.js HTTP Server

This repository demonstrates a common error in Node.js applications: unhandled errors within asynchronous operations.  The code simulates an HTTP server that performs an asynchronous task.  This task randomly fails, causing a 500 error without proper error handling.

The `bug.js` file shows the problematic code, while `bugSolution.js` presents a solution.

## How to reproduce

1. Clone this repository.
2. Run `node bug.js`.
3. Refresh the page several times. You'll observe that the server randomly returns a 500 Internal Server Error.

## Solution

The `bugSolution.js` file showcases the corrected code with proper error handling. It uses a `try...catch` block within the asynchronous operation to handle potential errors gracefully.