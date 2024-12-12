# Express.js JSON Body Parsing Issue

This repository demonstrates a common issue encountered when working with JSON request bodies in Express.js applications. The problem arises when the request body is either empty or contains invalid JSON data, leading to unexpected behavior or errors.

## Problem Description

The provided Express.js application utilizes the `express.json()` middleware to parse incoming JSON data. However, if the request body is empty or contains malformed JSON, the application might not handle this gracefully, resulting in errors or unexpected behavior.  This is especially true when expecting specific JSON structures.

## Solution

The solution involves adding error handling mechanisms to gracefully manage situations where the JSON parsing fails.  This approach ensures that the application doesn't crash and provides a more robust user experience.

## How to Run

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install necessary packages.
4. Run `node bug.js` to start the server with the buggy code.
5. Run `node bugSolution.js` to start the server with the fix.
6. Send test requests using tools like Postman or curl.  Try sending an empty body or a body with invalid JSON.