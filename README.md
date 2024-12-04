# Express.js JSON Body Parsing Issue

This repository demonstrates a common issue encountered when working with JSON request bodies in Express.js applications. The problem arises when the `express.json()` middleware fails to correctly parse the incoming JSON data, resulting in an empty `req.body` object.

## Bug Description

The provided `bug.js` file contains a simple Express.js server that attempts to handle POST requests containing JSON data. Despite the inclusion of `app.use(express.json())`, the server consistently logs an empty `req.body`, preventing proper access to the submitted data.

## Solution

The solution, found in `bugSolution.js`, addresses this issue by ensuring the correct configuration and handling of the JSON middleware and the potential causes like incorrect content-type header or body limits.