# Unhandled Exception in Dart Asynchronous Operation

This repository demonstrates a common, yet easily missed, error in Dart asynchronous programming: failing to re-throw exceptions caught in an `async` function's `catch` block.

The `bug.dart` file shows the problematic code.  The `catch` block only prints the error to the console, preventing higher-level error handling.

The `bugSolution.dart` file provides the corrected version. It demonstrates how to re-throw the exception using `rethrow`.