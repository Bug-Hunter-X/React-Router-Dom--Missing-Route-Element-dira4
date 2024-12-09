# React Router Dom: Missing Route Element
This example demonstrates an uncommon error in React Router Dom v6 where a missing route definition leads to unexpected behavior.  The application works correctly for defined routes ('/' and '/about'), but will show an error or unexpected behavior if the user tries to navigate to a path not included in the Routes component, such as '/contact'.

**Problem:** Missing Route elements for specific paths result in the application failing to render the intended component or throws an error. This is especially difficult to debug if the application doesn't have proper error handling or logging. 

**Solution:**  Ensure you define a Route for every path that should be handled by your React Router application. A catch-all route using `*` can be used for handling undefined routes.

See bug.js and bugSolution.js for detailed code examples.