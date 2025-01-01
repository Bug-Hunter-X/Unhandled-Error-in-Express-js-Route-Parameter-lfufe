# Unhandled Error in Express.js Route Parameter

This repository demonstrates a common error in Express.js route handlers: failure to handle invalid input parameters.  Specifically, the `/users/:id` route does not properly handle cases where the `id` parameter is not a valid number or is missing entirely.

## Bug

The `bug.js` file contains an Express.js application with a route that attempts to find a user by ID.  However, it lacks error handling to gracefully deal with invalid or missing `id` parameters. This can lead to unexpected behavior, crashes, or security vulnerabilities.

## Solution

The `bugSolution.js` file provides a corrected version of the route handler.  It includes comprehensive error handling to validate the `userId` and return appropriate error responses (400 Bad Request or 404 Not Found) when necessary. This ensures that the application behaves predictably and securely, regardless of the input provided.