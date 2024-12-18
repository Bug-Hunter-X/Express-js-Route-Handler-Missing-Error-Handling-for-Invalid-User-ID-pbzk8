# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid input.  Specifically, the provided code attempts to access user data based on a dynamically provided ID, but fails to check if the ID is a valid integer before parsing it. This can lead to unexpected errors and crashes if a non-numeric value is supplied.

The `bug.js` file contains the erroneous code, while `bugSolution.js` shows the corrected version with robust error handling.  The solution implements validation to ensure the ID is a number before attempting to parse it and subsequently handles the case where a user with the provided ID isn't found.